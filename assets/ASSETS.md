# Asset drop-in guide

## Sprites (replace procedural placeholders in code later)

Loader / texture keys:

| Key | File suggestion | Notes |
|-----|-----------------|-------|
| `bw_title` | `assets/img/bw_title.png` | Title |
| `bw_hit_only` | `assets/img/bw_hit_only.png` | Target only, no hole; 128×128; tintable |
| `bw_hole` | `assets/img/bw_hole.png` | Hole base 128×128; pivot center |
| `bw_bomb` | `assets/img/bw_bomb.png` | Bomb 128×128; do not tint |

W1 generates these procedurally in `src/assets/textures.ts`. When real PNGs arrive, load them under the same keys.

## Audio (paths already wired)

`public/assets/audio/`:

- `bgm_{01|02|03}_{100|120|140}.ogg`
- `sfx_hit.ogg` `sfx_perfect.ogg` `sfx_miss.ogg` `sfx_bomb.ogg`

Overwrite silent stubs with real files; no code change needed.
