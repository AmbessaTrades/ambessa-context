# The app on three surfaces

As of 13:20 EAT, 24 November 2026. "Exists" means a file was seen on the Mac by the writer of this page.

| | Web rooms | Mac app | Android APK |
|---|---|---|---|
| **Exists** | 19 rooms in `mockups/r2`, one parts kit, 750+ state pictures | Tauri v2 shell in `apps/juju-shell`, window 1440×900, icons, two commands | Android kit, minimum SDK 26, generated `gen/android` folder |
| **Does not exist** | Real data behind any room | A release build shown to anyone | **An APK file.** Any run on a phone |
| **Real now** | Clicks, states, the parts, the four skins | Loads skills; computes a card's reading time | nothing |
| **Next** | second review: eye, hands, fixer, whole-set director | rooms replaced by the round-2 rooms; crates wired in | one throwaway APK that makes one sound and plays it |

## Rules that hold on all three

1. Local PIN opens the app; it works offline.
2. Three doors only: Altar, Crossroads, Cauldron. The Tank is a chip at the top right of every room.
3. One primary button a room, always in the same place.
4. No key travels between devices. A key is checked on the device that makes the film.
5. At rest: at most 30 interface words at 1440, 24 at 390.
6. Skins: Nocturne (default), Codex, Atelier, Daylight.
7. The witch cat is the only character. It is Ambi's own logo, used as drawn.

## The phone, honestly

- Must: render films, make and judge sounds with Earshot, all with the Mac off (Said).
- Sound on the phone (Measured on the Mac only): without the speed loops 879 of 922 sounds match byte for byte; a 20 second rain loop took 48.8 s, 3.8 s with four loops
  rewritten in Rust; a 420 MB model set matched the Mac's on 18 of 18 clips.
- Cost (Estimated): 85 MB more APK, 420 MB of models beside it, 11 to 16 working days.
- Film drawing on the phone: no encoder code exists for Android. The brief's 580 MB memory ceiling is already broken on the Mac (432 MB to about 1 GB measured).
- No phone has been plugged in. Ambi was asked to plug in the Galaxy when he is home.

## Speed (Measured on a loaded Mac)

0.42 times real time against the brief's 4 to 8. Frames: 12 a second at load 22. Hardware encode of 120 frames 1.92 s, software 7.52 s. A speed job (chunks, reuse of finished
pieces, a lossless middle step) is running now.
