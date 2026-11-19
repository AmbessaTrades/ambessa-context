# 04 — Evidence

`outliers.csv` — every upload at 2x its channel's recent median or more, taken 19 Nov 2026 from each
channel's most recent uploads (24, or 30 for two channels whose video tab exposes nothing). Columns:
channel, the channel's median views, the title, the views, the ratio, the video id.

102 outlier rows across 26 channels. `channels.jsonl` holds the full sets including non-outliers.

Two caveats, stated because they change what the numbers mean:

- A ratio is only as good as its median. A Shorts channel's median makes a longform hit look enormous.
- Views are lifetime views at the moment of the scan, not views in the first week.

The thumbnails for every row are in `09-assets/library/`, captioned with the channel, the views and the
ratio.
