# Audio licenses — Beat Whack

All tracks below allow **commercial use in a game** (including YouTube Playables).  
Attribution is **not required** (CC0 / Kenney CC0); we list authors for good practice.

## BGM

| File | Title | Author | Source URL | License | License URL | Notes |
|------|-------|--------|------------|---------|-------------|-------|
| `bgm_01_100.ogg` / `_120` / `_140` | Empacotatron (loop) | Fupi | https://opengameart.org/content/empacotatron | CC0 1.0 | https://creativecommons.org/publicdomain/zero/1.0/ | Native tempo ~**167 BPM** (onset estimate). Trimmed to ~55s then `ffmpeg rubberband` tempo→100/120/140 (pitch preserved), export OGG Vorbis ~64 kbps, final clip ~50s. Source: `audio_sources/empacotatron_loop.ogg`. |
| `bgm_02_100.ogg` / `_120` / `_140` | Synthwave House Loop | Fupi | https://opengameart.org/content/synthwave-house-loop | CC0 1.0 | https://creativecommons.org/publicdomain/zero/1.0/ | Native tempo ~**112 BPM** (onset estimate). Full ~50.5s source; `rubberband`→100/120/140; OGG ~64 kbps; trim/fade to ≤50s. Source: `audio_sources/synthwavehouse.ogg`. |
| `bgm_03_100.ogg` / `_120` / `_140` | Trance Adventure | MintoDog | https://opengameart.org/content/trance-adventure | CC0 1.0 | https://creativecommons.org/publicdomain/zero/1.0/ | Author-labeled **140 BPM**. Took 55s from t≈8s; `rubberband`→100/120/140 (140 = identity); OGG ~64 kbps; ~50s. Source: `audio_sources/trance_adventure_bpm140.ogg`. |

## SFX

| File | Source clip | Author | Source URL | License | License URL | Notes |
|------|-------------|--------|------------|---------|-------------|-------|
| `sfx_hit.ogg` | `impactSoft_medium_001.ogg` | Kenney (Kenney.nl) | https://kenney.nl/assets/impact-sounds | CC0 1.0 | https://creativecommons.org/publicdomain/zero/1.0/ | From Kenney Impact Sounds pack. Re-encoded OGG ~96 kbps. |
| `sfx_perfect.ogg` | `confirmation_002.ogg` | Kenney (Kenney.nl) | https://kenney.nl/assets/interface-sounds | CC0 1.0 | https://creativecommons.org/publicdomain/zero/1.0/ | From Kenney Interface Sounds pack. |
| `sfx_miss.ogg` | `error_005.ogg` | Kenney (Kenney.nl) | https://kenney.nl/assets/interface-sounds | CC0 1.0 | https://creativecommons.org/publicdomain/zero/1.0/ | From Kenney Interface Sounds pack. |
| `sfx_bomb.ogg` | `impactMetal_heavy_002` + `zapThreeToneDown` | Kenney (Kenney.nl) | https://kenney.nl/assets/impact-sounds · https://kenney.nl/assets/digital-audio | CC0 1.0 | https://creativecommons.org/publicdomain/zero/1.0/ | Layered mix of Impact Sounds + Digital Audio packs for a longer punch. |

## Rejected sources (do not use)

| Source | Reason |
|--------|--------|
| Mixkit Stock Music Free License | Explicitly **disallows video games**. |
| Unclear / “royalty-free” without terms | Not verified — not used. |

## Processing

- Toolchain: `ffmpeg` 7.x with `rubberband` filter (tempo change, pitch preserved).
- Working copies and originals live under `/workspace/beat-whack/audio_sources/` (not shipped in Playables initial pack unless copied into `public/`).
- Runtime game assets: `public/assets/audio/` (mirrored to `assets/audio/`).

Last updated: 2026-10-13 (HKT)
