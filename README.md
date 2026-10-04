# konsoll-site

Public site and (from v0.9.0) beta download host for **KONSOLL** — a four-module multi-FX instrument by Fløa (AU / VST3).
Live (once published): <https://floamusic.github.io/konsoll-site/> · all instruments: <https://floamusic.github.io/>

| Path | What it is |
| --- | --- |
| `index.html` | Home — modules, what moves, get the beta (SOON), support and contact |
| `assets/css/site.css` | Single stylesheet in the plug-in's Soft Strata palette |
| `assets/fonts/` | Geist Mono (SIL OFL, licence included) |
| `assets/img/` | Interface renders from the product repo (`Konsoll_DSPTests --render-promo <file> [preset]`, 2x, footer cropped so no version is pictured) and the wordmark |

Static HTML/CSS, no build step, nothing from a CDN. The product source is private (`floamusic/Konsoll`); nothing here is generated from it.

## Releases (to come)

Binaries are not in this repo; they go on its GitHub Releases, as for FLOATING (`floating-site`):
`Konsoll-<version>-macOS-arm64.pkg` plus a byte-identical `Konsoll-macOS-latest.pkg` that the site links through `/releases/latest/download/`, and `SHA256SUMS.txt`. **Never mark a release as pre-release** — `/releases/latest/` would stop seeing it.

The plug-in's Check for updates will open `https://floamusic.github.io/konsoll-site/updates.html?v=<version>&os=mac`; once that ships, `updates.html` must never move.
