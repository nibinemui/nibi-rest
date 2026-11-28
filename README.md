# Unova Online website

The website for Unova Online, the online layer for Pokémon Black and White. It is a single static page in `public/` (`index.html` and `images/`). `server.js` is only for previewing it locally.

## Run it locally

Requires Node.js 20 or newer. Run `npm start` and open http://localhost:3000.

## Hosting

Cloudflare Pages, connected to this repo's `unova-online` branch: no build command, build output directory `public`. Every push to the branch deploys. The custom domain `unovaonline.nibi.rest` is added on the Pages project (nibi.rest's DNS is on Cloudflare, so the record is made automatically). `public/_headers` sets security headers and caches images for a day.

## Images

All artwork lives in `public/images/`. The screenshots are taken from Unova Online running the original games, scaled up with nearest-neighbour so the pixels stay sharp (the page also sets `image-rendering: pixelated`).

| File | What it shows |
| --- | --- |
| `accumula-trainers.png` | Twelve trainers with name tags in Accumula Town (hero) |
| `instances.png` | Switching copies of Unova from the C-Gear |
| `social.png` | Trainers in town and the C-Gear chat |
| `trading.png` | The GTS room and menu |
| `battles.png` | The talk-to-player menu and a link battle |
| `missions.png` | The C-Gear Missions page |
| `trainer-looks.png` | The Looks shop |
| `shiny-announcement.png` | A shiny wild Pokémon and its chat announcement |
| `cgear-home.png` | The C-Gear home screen |
| `unova-online-logo.png`, `favicon.png` | The Unova Online logo |

To replace a picture, overwrite the file with one of the same aspect ratio (feature cards are 520:192, two DS screens side by side). Pokémon and related names are trademarks of their respective owners; this is a fan project.
