<!-- copied from the Juju repo: docs/earshot-phone-spike.md, last changed 08:23 EAT, 24 Nov 2026. Private lines removed. Do not edit here. -->
> Working document. Subject to change through continued conversation. Nothing here is a requirement until Ambi says so.

# Earshot on the phone: feasibility spike (24 Nov 2026)

**Question.** Can Earshot run on a Samsung Galaxy S20/S21 (Android arm64, about 8 GB RAM) inside a Tauri v2 app with the Mac switched off? That means all of it: making sounds, building new ones, and listening to judge them.

**Owner's words (24 Nov 2026):** "for the APK version, it needs to somehow use earshot as well, independent of my computer" and "all aspects of earshot are important to use".

**Tags.** Every claim carries one of three tags:
- **[M]** measured on this Mac in this spike.
- **[S]** read in source (Earshot's code, a package index, a vendor page).
- **[E]** estimated.

No phone was attached and no Android emulator is installed (the T3 device list reports "Android SDK was not found"), so nothing below ran on Android.

**The Mac.** M1, 8 cores, 16 GB RAM. Swap was 5.5 to 8 GB used during the spike. A LOT render (ffmpeg plus loopframe) ran in parallel for part of it, and the load average reached 19 to 30. Timings marked *clean* come from the first bench run, at load about 3. The others are inflated two to three times by contention. Every heavy job ran under `nice -n 15` or `nice -n 19`.

Earshot source: `.toolchain/earshot/src` at commit `7a7f7c5`, release 1.0.0, MIT. Scratch files, scripts and raw results: `(scratch) These live in temporary space and a reboot can clear them.

---

## 1. Making sounds without models and without numba

**The lite venv** is at `.toolchain/earshot/lite`. It runs Python 3.13.7 with numpy 2.5.5, scipy 1.18.1, soundfile 0.14.0 and soxr 1.1.0 (plus cffi, pycparser and typing-extensions, which those pull in). numba is absent: `import numba` raises ImportError. It takes 98 MB on disk. **[M]**

These versions are the same as the Android wheels found in section 4a, except numpy is 2.5.5 here and 2.5.4 there. So this Mac test is a close stand-in for the phone's Python layer. **[M]/[S]**

**Result: `earshot make` works for all 8 sounds without numba, and the output is byte-identical to the numba output.** Every WAV, both seeds, compared sample by sample: maximum difference 0.0. **[M]**

The catalogue agrees too. Each design was rendered at seed 3 in the full venv and in the lite venv and compared by audio hash. **[M]**
- **879 of 922 designs were compared, and all 879 are identical.** There were no errors. That covers all 873 one-shots except four, plus 9 of the 49 loops.
- Four designs passed 60 CPU s in lite and were stopped: `rain/roof`, `riser/air`, `riser/swell`, `riser/tension`.
- 39 loops were not run without numba, because at lite speed each takes minutes. The 20 s and 8 s rain loops above are identical.

Clean bench, one process per sound. *First* is the first make in a fresh process. *Again* is a second make in the same process.

The *Made from* column comes from the replay count in section 4b. "Learned" means one of the 309 designs learned from recordings. "Replays learned data" means other code that calls the learned resynthesis. "Code synthesis" means made by code alone.

| Sound (request) | Design chosen (made from) | Length | Lite first / again (s) | numba cold / warm-cache first / again (s) | Peak RSS lite / numba (MB) | WAV size |
|---|---|---|---|---|---|---|
| UI tap ("a soft ui tap") | keyboard/mechanical (learned) | 0.29 s | 3.69 / 0.09 | 1.49 / 0.60 / 0.07 | 175 / 230 | 83 KB |
| Footstep ("a footstep on gravel") | step/pebbles (learned) | 0.51 s | 3.33 / 0.09 | 1.32 / 0.64 / 0.07 | 183 / 247 | 148 KB |
| Page turn | page/turn (learned) | 0.96 s | 3.48 / 0.34 | 1.40 / 0.71 / 0.24 | 292 / 331 | 276 KB |
| Door ("a wooden door closing") | door/shut (learned) | 1.81 s | 3.30 / 0.39 | 1.47 / 0.77 / 0.28 | 354 / 404 | 522 KB |
| Rain loop ("rain on a window, loop", 20 s) | rain/window (**code synthesis**) | 20.0 s | **48.8 / 54.0** | 3.03 / 2.16 / 1.47 | **1008 / 1111** | 5.76 MB |
| Whoosh ("a fast whoosh") | whoosh/fast (replays learned data) | 0.24 s | 0.54 / 0.07 | 0.45 / 0.47 / 0.07 | 188 / 203 | 68 KB |
| Low drum ("a low drum hit") | kick/soft (replays learned data) | 0.94 s | 1.64 / 0.23 | 1.35 / 0.68 / 0.18 | 262 / 312 | 270 KB |
| Chat pop ("a chat message pop") | receive/cork (replays learned data) | 0.41 s | 2.98 / 0.10 | 1.30 / 0.68 / 0.08 | 210 / 267 | 118 KB |

All 8 sounds passed Earshot's own audit as clean. **[M]** The WAVs are 24-bit stereo at 48 kHz. **[M]**

- Importing earshot takes about 1.5 s in lite and 0.75 s with numba. **[M]**
- An 8 s rain loop under load: lite 81 s; numba 5.2 s first, 2.2 s again; peak RSS 473 MB lite, 574 MB numba. **[M]**
- Whole catalogue with numba: all 922 designs render with no errors in 671 s total, median 0.24 s, slowest `fire/camp` at 21 s. 890 of the 922 pass the audit clean; the 32 others carry the audit's own warnings. **[M]**
- Lite whole-catalogue sweep: 1,580 CPU s for the 879 designs compared, against 376 s with numba for the same designs. **[M]**
  - One-shots without numba: median 0.48 CPU s, 90th percentile 4.0 s, 64 over 5 s, 24 over 10 s; slowest `riser/shepard` at 59 s, plus the four stopped at 60 s.
  - Part of this sweep ran on efficiency cores under `taskpolicy -b` during a LOT render, so these times are upper bounds.
- **Which kernels matter [M]:** 162 of the 879 designs call no numba kernel. The most used kernels are `fx._allpass` (594 designs), `fx._release` (230), `dsp._svf` (167), `fx._fdn` (128), `fx._follow` (50), `dsp._osc` (35), `dsp._blep` (34) and `texture._rings` (25). These 8 cover nearly all the use.

**Why the first sound is slow and later ones are fast.** Most of the "first" cost in lite is one reverb impulse response, built once per process by `forge/fx.py:_fdn`: 2.6 s of 2.8 s for the tap, by cProfile. **[M]** On the phone, one long-lived Python process keeps that cost to app start.

**What really needs numba is a few event loops.** The profile of the 8 s rain loop: `synth/texture.py:_rings` 11.9 s plus `_bursts` 5.0 s, out of 17.6 s. **[M]**

### The calls that use numba

There are 28 `@njit` kernels, 570 source lines in total. **[S]**

- `forge/dsp.py`: `_svf`, `_blep`, `_osc`
- `forge/fx.py`: `_allpass`, `_fdn`, `_follow`, `_rise`, `_release`
- `forge/recipes/impact.py`: `_vcomb_core`
- `synth/chip.py`: `_bl_render`, `_pulse_steps`, `_stair_steps`, `_lfsr_steps`, `_delta_steps`
- `synth/drums.py`: `_follow`
- `synth/strings.py`: `_past`, `_hammer_force`
- `synth/texture.py`: `_rings`, `_bursts`
- `synth/voice.py`: `_add`, `_advance`, `_voice`, `_soft`, `_ladder`, `_feedback`, `_tap`, `_echo`, `_allpass_chain`

**A fallback exists, and it is the code's own.** `forge/dsp.py:146-150` and `forge/recipes/impact.py:281-285` catch the failed `from numba import njit` and replace `njit` with a decorator that does nothing. Every kernel then runs as plain Python on numpy arrays. No other module imports numba. `pyproject.toml` says so itself: "without it they run in plain Python". **[S]**

**Proof that the kernels can be replaced.** Four kernels were rewritten as a throwaway Rust `cdylib` (`k.rs`, about 45 lines; `_rings`, `_bursts`, `_allpass`, `_fdn`) and patched in over ctypes, in the lite venv. **[M]**
- Output is byte-identical to numba on tap, 20 s rain, door and pop.
- The 20 s rain loop dropped from 48.8 s (lite, clean) to 3.8 s (Rust, under load), against numba's 2.2 s first / 1.5 s again.
- The macOS dylib is 410 KB.

**Phone time [E].** Assumed: the S20 (Snapdragon 865 or Exynos 990) and S21 (Snapdragon 888) are about 0.5 to 0.65 of an M1 performance core on one thread, from public single-core benchmark figures, not measured here. So multiply Mac times by 1.5 to 2.
- A one-shot with Rust kernels: about 0.15 to 0.8 s.
- The 20 s rain loop: about 3 to 8 s with Rust kernels, about 75 to 100 s without them.

---

## 2. `build`, recipes and `fit` without the listening models

| Command | Lite venv (no models, no numba, no ffmpeg on PATH) | Missing on the phone, and the fix |
|---|---|---|
| `make` to WAV or FLAC | works **[M]** | nothing |
| `make` to OGG, MP3, M4A or WebM | fails: "writing .ogg needs ffmpeg on PATH" **[M]** | `master.write` calls the ffmpeg program. libsndfile writes OGG Vorbis and Opus itself (the Mac sweep wrote both through soundfile **[M]**), and the Android libsndfile build carries Vorbis, Opus, mpg123 and LAME **[S]**. Changing the write path is about 15 lines **[E]**. |
| `recipe --list`, recipe render | works (99 recipes) **[M]** | nothing |
| `build "…"` | **works, with "no ears"** **[M]**. Hail on a tin roof: 62 s CPU, **1.59 GB peak RSS**. A whale singing: 132 s CPU, 824 MB. A robot arm: 19 s CPU, 593 MB. Each run used 8 tuning rounds under load. | The tuner can then only keep the sound clean and near the asked length; its own note says "tuned in 8 rounds: no change scored better … a person should listen once". The draft step falls back from the atlas to the word reader. Memory needs watching on 8 GB. |
| `fit` (Python call `auto.fit(array)`) | **works** **[M]**. tap: sines, 20 CPU s. footstep: modal, 33 s. page: modal, 37 s. Peak 348 to 566 MB. No numba and no librosa were loaded. | nothing for the core fit |
| `fit FILE` (command line) | fails twice **[M]**. File decoding (`audio.load`) runs the `ffmpeg` program even for a WAV, and the PNG step wants matplotlib. | Read WAV, FLAC and OGG through soundfile (about 10 lines) and skip the picture **[E]**. Matplotlib and Pillow Android wheels exist (section 4a). |
| `sfx check FILE`, `pack` | fail: ffmpeg **[M]** | same `audio.load` change |
| `measure` | fails: needs librosa **[M]** | librosa requires numba ≥ 0.61 **[S]**, and no numba wheel exists for Android on Python 3.10 or newer (section 4a). Port the handful of librosa calls it uses (onsets, chroma, HPSS, yin, beat tracking) or drop `measure` **[E]**. |
| `describe`, `match`, `realness`, `compare`, `timeline`, `critique`, `make --listen`, build with ears | refuse with one sentence naming torch, transformers and librosa **[M]** | section 3 |

**Package needs on the phone:**
- make, recipes, build without ears, fit: numpy, scipy, soundfile with libsndfile, soxr, cffi, pycparser, typing-extensions. **[S]/[M]**
- The 28 numba kernels: a native replacement, for speed only. **[M]**
- Images: matplotlib and Pillow. **[S]**
- MCP server, the CLI and requests: not needed on a phone app.

---

## 3. The listening models

### Files on disk

These files sit in `.toolchain/earshot/src/.cache/hf`. That folder is 1.0 GB, with 17 MB of decode cache and 4.6 MB of embedding cache beside it. **[M]**

| Model | Weights file | Bytes | Parameters (from the safetensors header) |
|---|---|---|---|
| CLAP `laion/larger_clap_general` @ `16c8cc3` | model.safetensors | 776,327,440 | 194.0 M: audio tower (HTSAT) 67.9 M, text tower (RoBERTa) 124.6 M, two projections 1.4 M **[M]** |
| AST `MIT/ast-finetuned-audioset-10-10-0.4593` @ `f826b80` | model.safetensors | 346,404,948 | 86.6 M (86.2 M transformer, 0.4 M classifier over 527 classes) **[M]** |

**Correction to the ADR.** The two models take **1.12 GB on disk** (about 1.1 GB with tokenizer and config files). The README's and ADR 0001's "about 2.2 GB on disk" is not what this cache holds. The size is measured **[M]**; where the 2.2 GB figure comes from is unknown.

### What each model computes

- **CLAP audio tower.** A 64-band mel image of a 10 s window (shorter sounds are repeat-padded) becomes a 512-number vector. It is used by the atlas (`sounds/atlas.py`), by build's ears (fit z, nearest designs, the realness CLAP head) and by describe, match and compare. **[S]**
- **CLAP text tower.** Words become a 512-number vector. It is used for the request, the 322 vocab terms and the atlas text. Text vectors are cached on disk. **[S]**
- **AST.** A 1024×128 filter-bank image at 16 kHz becomes 527 AudioSet class probabilities. It is build's "second ear" (whether the sound is music, speech or a synth tone) and `realness --ast`. **[S]**
- **Realness.** A plain-JSON logistic model over the CLAP embedding: 512 coefficients, the signal head weighted 0 by its own fit. No extra network. **[S]**
- **The atlas.** `data/sounds_atlas.npz`, 1.7 MB, holds the audio and text vectors of all 922 designs, already computed. **[S]** So ranking the catalogue needs only the text tower, and judging a new render needs the audio tower.

### A smaller form is realistic, and was measured

Public int8 ONNX exports of both models exist (Hugging Face `Xenova/larger_clap_general`, `Xenova/ast-finetuned-audioset-10-10-0.4593`). They were downloaded and run with onnxruntime 1.32 on the Mac, against the pinned torch fp32 models, on the 16 rendered WAVs from section 1 plus 2 more: 18 clips and 12 texts. **[M]**

| Model form | File size | Fidelity against fp32 torch | One forward pass on the Mac (4 threads, under load) | Peak RSS |
|---|---|---|---|---|
| CLAP audio int8 | 78.2 MB | cosine ≥ 0.998 (mean 0.999). Best text on all 18 clips the same. Same nearest atlas design on 18/18. Realness head p_real within 0.067. | 0.78 s per clip (torch fp32: 0.56 s) | 294 MB |
| CLAP audio fp16 | 143.4 MB | cosine ≥ 0.99999 | 1.6 s | 601 MB |
| CLAP text int8 | 126.6 MB | cosine ≥ 0.976 (mean 0.989), one text at a time. Padded batches break it, because this export has no attention-mask input. With both towers int8: top text the same on 15/18; per-sound z off by 0.10 on average, at most 0.40. | 0.06 s per text | 265 MB |
| CLAP text fp16 | 251.0 MB | cosine ≥ 0.999999. With audio int8 + text fp16: top text the same on **18/18**; per-sound z off by 0.02 on average, at most 0.07. | 0.12 s per text | — |
| AST int8 | 90.8 MB | top class the same on 18/18; class probability off by at most 0.12 | 3.1 s per 10 s clip (torch: 2.6 s) | 489 MB |
| Parameter-count check | | 194.0 M + 86.6 M parameters at 1 byte each comes to about 281 MB, against 296 MB measured as files | | **[E]→[M]** |

**Total listening weights: 296 MB all int8, or 420 MB with the text tower in fp16** (78.2 + 251.0 + 90.8), against 1.12 GB fp32. **[M]**

The 18 clips and 12 texts are a small sample; read these as early evidence, not a validation.

**Recommended set: CLAP audio int8, CLAP text fp16, AST int8 (420 MB).** All-int8 text lets the per-sound z move by up to 0.40. Build's verdict needs a lead of 1.0 over the design `make` would hand over, so that drift is large enough to matter. **[M]**

**Text-tower drift [M].** The drift comes from the int8 text tower. Precomputing the fixed text (322 vocab terms, atlas text) does not help the owner's own request, which goes through the text tower live. fp16 removes the drift (measured above).

**Not ported yet [S].** The mel front ends live in transformers' `ClapProcessor` and `ASTFeatureExtractor`. They are numpy-level code, about 100 lines together **[E]**, and must match within float tolerance. The tokenizer is RoBERTa BPE: the `tokenizers` Android wheel or the Rust `tokenizers` crate.

### What judgement remains with no model at all [S], [M]

- **The audit on every render** (`forge/sfx.check`), code only:
  - silent, clicks and edge discontinuities, clipping, DC offset;
  - a metallic ring in the tail, a truncated tail, digital silence, a tail that rises again;
  - the rising-glide "synth whip" tell;
  - stacked hits and pre-swell.
- **build's `measures`:** length, hit time, onset, active time, brightness (spectral centroid), onset density, each compared with the asked length and the nearest real design.
- **fit's `quality.score`:** mel distance, tone, envelope, onset, and excess or missing energy against the original.
- **What is lost:** whether it *sounds like* the words (z), recorded versus synthesized (p_real), what it is heard as, the AudioSet second opinion, and the tuner's search for a better fit. In Earshot's own words without ears: "measured, not heard".

---

## 4. Phone options

### (a) Embed CPython (Chaquopy) and run Earshot itself

**Wheels on the live package indexes, checked 24 Nov 2026 [S]:**

| Index | numpy | scipy | soundfile | soxr | Python versions |
|---|---|---|---|---|---|
| PyPI | no Android wheels | none | none | none | (cffi 2.1.1 has iOS wheels only) |
| Chaquopy `chaquo.com/pypi-13.1` | 1.26.2 (cp39–cp313) | **1.8.1 newest** (cp39/cp310), below Earshot's `scipy>=1.11` | 0.13.1 (cp310) | 0.4.0 (cp313), 0.3.7 (cp311/312) | cffi 1.17.1 (cp313); `chaquopy-libsndfile` 1.0.28 |
| Chaquopy `chaquo.com/pypi-upstream` (unofficial, per its maintainer, 27 Jul 2026, issue #1237) | 2.3.2 (cp313) | 1.16.1 (cp313) | none | none | cp313 |
| **Flet `pypi.flet.dev`** | **2.5.4** | **1.18.1** | **0.14.0** (libsndfile 1.2.2 inside, with Vorbis, Opus, mpg123, LAME) | **1.1.0** | **cp312, cp313, cp314**, tag `android_24_arm64_v8a` |

Flet also carries cffi 2.1.1, onnxruntime 1.32.0, tokenizers 0.23.3, scikit-learn 1.9.1, msgpack, matplotlib 3.11.2, Pillow 13.0.0 and safetensors 0.8.0. **[S]**

**A fallback set at cp313, built from Chaquopy's own two indexes [S], untested:**
- numpy 2.3.2 and scipy 1.16.1 from `pypi-upstream`;
- soxr 0.4.0 and cffi 1.17.1 from `pypi-13.1`;
- soundfile as its pure-Python PyPI wheel (0.14.0, `py2.py3-none-any`) over `chaquopy-libsndfile` 1.0.28.

All of these meet Earshot's version floors. Two things are not verified: whether soundfile's `find_library` finds Chaquopy's libsndfile, and whether that old libsndfile writes Opus. Byte identity with this set is also not tested. Use it if Flet's wheels will not load under Chaquopy.

No index carries **numba, llvmlite, torch or librosa** for Python 3.10 or newer. Chaquopy has numba 0.48 and torch 1.8.1 only for cp38, which Chaquopy 17 dropped. **[S]**

**The Flet wheels themselves [M]**, downloaded and read with the NDK 27 `llvm-readelf`:
- **Compressed size:** numpy 7.1 MB (23.2 MB unpacked), scipy 29.6 MB (84.2 MB unpacked), soundfile 0.02 MB, libsndfile 1.0 MB, soxr 0.19 MB, cffi 0.2 MB, libc++_shared 0.4 MB.
- **Loading:** the `.so` files need only `libpython3.13.so`, `libc++_shared.so` and system libraries. OpenBLAS is linked statically; the 17.7 MB `flet-libopenblas` wheel is a build-time `.a` file and is not needed at runtime. LOAD segments are 16 KB aligned.
- **How soundfile finds libsndfile:** Flet patched soundfile to look in the wheel's `opt/lib` on Android.

**Chaquopy 17.2 (26 Oct 2026, MIT licence) [S]:**
- It supports Python 3.10 to 3.15, Android Gradle plugin 7.3 to 9.5 and minSdk 24, in an app module or exactly one library module.
- Since 17.0 it takes `--extra-index-url`.
- Its changelog: "Improved compatibility with various ways of bundling non-Python libraries in a wheel" and "Improved compatibility with various ways of tagging a wheel as Android-specific".

**Fit with Tauri v2 [S]:**
- `tauri-cli` v2.12.6's Android template uses Android Gradle plugin 9.3.1, Gradle 9.6.1, minSdk 24 and a `com.android.application` app module, all inside Chaquopy's range.
- A public Tauri 2 + Chaquopy app exists and ships: `kernelPani/Nuclear_Mobile`, AGPL. It runs yt-dlp through Chaquopy; its universal release APK is 79.8 MB. Its pattern:
  - `id("com.chaquo.python")` is added to `gen/android/app/build.gradle.kts`, with `abiFilters += "arm64-v8a"`;
  - a Kotlin `@TauriPlugin` calls `Python.getInstance().getModule(...).callAttr(...)` from a Tauri `@Command`.
- **Not proven:** that Chaquopy loads Flet's `opt/lib` libraries (libsndfile, libc++_shared). The fallback is to copy those two `.so` files into `jniLibs/arm64-v8a`. This is the first risk to retire.
- **Other route:** python.org now publishes an Android embeddable package (3.14.10: 23.0 MB tar.gz). With PyO3 and Flet's cp314 wheels, that avoids Kotlin and Chaquopy. No known Tauri example; more glue work.

**APK size added [M]/[E]:**

| Part | Size | Tag |
|---|---|---|
| Python runtime (Chaquopy target 3.13.16: 7.3 MB native + 4.3 MB stdlib) | about 11.6 MB | [M] |
| numpy, scipy, soundfile, soxr, cffi and the native libraries, compressed | about 38.5 MB | [M] |
| Earshot code and data, zipped (the data folder alone is 31.6 MB) | 33.1 MB | [M] |
| Rust kernels | about 1 MB | [E] |
| **Total for make, build without ears, recipes and fit** | **about 85 MB** | [E] |
| Listening models, recommended set (CLAP audio int8 78.2, CLAP text fp16 251.0, AST int8 90.8); 296 MB if all int8 | 420 MB | [M] |
| onnxruntime (Flet Python wheel; the official Android AAR is 59.3 MB for all ABIs) | about 10 MB | [M] |
| **Total with all of Earshot including ears** | **about 515 MB** (about 390 MB all int8) | [E] |

On the phone itself, Python packages are unpacked, so they take more room than the APK figures: numpy and scipy alone are about 107 MB unpacked. **[M]**

**Fitting the big build onto the phone [E].** Google Play caps a base APK at 200 MB, but a sideloaded APK has no such cap. Two choices:
- Ship the models as a one-time file copied onto the phone from the Mac or a local file.
- Shrink the AST to its q4 export (60 MB, fidelity not measured).

**Work, in days [E]:**

| Step | Days |
|---|---|
| Chaquopy into the Tauri `gen/android` project, Flet index, a Kotlin `@TauriPlugin` bridge, the libsndfile and libc++ loading check | 2–3 |
| Rust kernels for all 28 `@njit` functions, with a parity test against numba hashes over all 922 designs (the sweep harness exists) | 3–4 |
| ffmpeg removed from `audio.load` and `master.write` | 0.5 |
| The listening models on onnxruntime: CLAP audio and text, AST, the two mel front ends, the tokenizer, parity tests | 4–6 |
| `measure` without librosa | 1–2 |
| **Total** | **about 11–16 working days** for every part of Earshot |

**Lost:** almost nothing.
- `earshot mcp`, ffmpeg video reading, and Gemini critique without a network are not needed on a phone.
- Small drift from int8 (measured above).
- Earshot upgrades are drop-in: it is Earshot's own Python.

**Memory risk [M].** One build peaked at 1.59 GB in a single process, and the 20 s rain at 1.0 to 1.1 GB. On 8 GB phones with Android's per-app limits this is tight but likely to fit [E]. Load the models one at a time and free them after a job.

### (b) Port only the render path to Rust

**Code lines (code only, no docstrings or comments, counted by AST) [M]:**

| Part | Lines |
|---|---|
| Replay core: `synth/resyn.py` 703, `synth/quilt.py` 357, `sounds/learned.py` 283, `synth/perform.py` 256, `synth/master.py` 152, `sounds/registry.py` | 1,974 |
| …of which the resyn render functions alone (32 functions) | 413 |
| Shared filters and reverb: `forge/dsp.py`, `fx.py`, `polish.py`, `sfx.py` (the audit) | 1,795 |
| Recipe engine (`recipe.py`) | 844 |
| Words to design (`brief.py`, `sounds/lexicon.py`, `make.py`) | 3,645 |
| Code-synthesized designs (70 files) | 20,663 |
| `build.py` | 1,434 |
| `fit` | 5,947 |
| **All of Earshot** | **46,789** |

**scipy and numpy calls to replace [S]:**
- FFT (rfft, ifft, irfft), `next_fast_len`, `signal.resample_poly` and `resample`, STFT and ISTFT;
- `ndimage.uniform_filter1d`, `maximum_filter1d`, `gaussian_filter`, `binary_dilation`, `median_filter`, `convolve1d`;
- `linalg.svd`;
- elsewhere: `fftconvolve` (34 uses), `butter`, `sosfilt` and `lfilter`.

**Coverage of learned replay [M].** Rendering every design with `resyn.render` made to raise showed:
- 309 learned designs plus 191 others whose code calls `resyn.render` (textures, drums, notes and the rest), so **500 of 922 designs replay learned data**;
- 422 designs are pure code synthesis;
- the learned designs cover 228 of 384 families;
- **50 of 99 cookbook recipes** use learned parts only; the rest also need parts like `rumble/quake`, `wind/window`, `tick/wood`, `door/slide` and `fire/camp`.

**What a Rust port means [E]:**
- Replaying learned designs from the 34 MB data folder plus recipes: about 4,600 Rust lines (replay core, dsp and fx, recipe engine), about 15–25 days.
- Picking a design from words: another 3,600 lines.
- Exact numpy random-stream parity (PCG64) is needed to match takes; otherwise takes differ but stay valid.

**Size added:** about 35 MB (data plus a small binary). **[E]**

**Lost:** 422 code designs, `fit` (5,947 lines), `build`'s tuner unless also ported, the listening models (they would need `ort` in Rust anyway), and every future Earshot update (a fork to maintain). This does not meet "all aspects of earshot".

### (c) Ship every design pre-rendered, plus recipes replayed in Rust

All 922 designs were rendered once, at seed 3, and encoded through libsndfile. **[M]**
- **FLAC 16-bit:** 186.0 MB.
- **OGG Vorbis:** 33.4 MB (one-shots 22.0 MB, 49 loops 11.4 MB).
- **Opus:** 33.0 MB.
- Three takes each in Vorbis would be about 100 MB. **[E]**

The Rust part is about 1,500 lines (recipe engine plus pitch, filter and placement) for about 6–10 days. **[E]**

**Lost:** new takes, length, pitch and feel controls on each design (a pitch shift of a file is not a re-render), `fit`, `build`'s search, and listening. Recipes would layer fixed files. This is a catalogue player, not Earshot.

### (d) The Mac makes, the phone plays

The owner rejected this ("independent of my computer"). It is listed only as the fallback if a phone path fails. It adds 0 MB to the APK, and with Mac Earshot unchanged it takes 0 days. **[S]**

---

## 5. Recommendation

1. **Pick (a): embed CPython with Chaquopy and run Earshot's own Python on the phone.** The phone's Python packages exist on Flet's index at the versions tested here (numpy 2.5.4, scipy 1.18.1, soundfile 0.14.0, soxr 1.1.0, Python 3.13). Without numba, Earshot rendered 879 of 922 designs byte-identically, with no errors. The four slowest were stopped at 60 s and 39 loops were not run. **[M]**
2. **Put Rust where it pays: replace the 28 numba kernels (570 lines) with a Rust library**, starting with the 8 that nearly all designs use. This spike's 4-kernel Rust test was byte-identical and cut the 20 s rain loop from 48.8 s to 3.8 s. Everything else stays Python glue. **[M]**
3. **Give it ears on the phone with ONNX: 420 MB** (CLAP audio int8, CLAP text fp16, AST int8). On 18 clips and 12 texts it agreed with the Mac models: same best text 18/18, same nearest design 18/18, same AudioSet top class 18/18, z within 0.07. An all-int8 text tower saves 125 MB, but only 15/18 then match. **[M]**
4. **Expected size and work [E]:** about 85 MB of APK for make, build, recipes and fit, plus 420 MB of model weights shipped as a side file. About 11–16 working days for all of Earshot. Watch the 1.6 GB peak of one build. Nothing here ran on Android yet.
5. **Build first: a throwaway Tauri v2 Android APK** with the Chaquopy plugin and `--extra-index-url https://pypi.flet.dev`. It calls `earshot.make.make("a soft ui tap", ".../tap.wav")` through a Kotlin `@TauriPlugin` and plays the file. It retires the one unproven link: Chaquopy loading Flet's libsndfile and libc++. If Flet's wheels will not load, try the Chaquopy-only cp313 set in 4a.
