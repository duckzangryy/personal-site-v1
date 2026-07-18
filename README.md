# personal-site-v1 — vanhcutii personal site

Early personal landing page for **Vương Việt Anh** — lock-screen intro, anime aesthetics, music, and interactive widgets. Static HTML/CSS/JS, no build step.

> Historical site (vanhcutii.store era). See also [Portfolio-1](https://github.com/duckzangryy/personal-portfolio) and [ProfileWeb](https://github.com/duckzangryy/profile-web) for later iterations.

## Features

- Full-screen lock / welcome layer with video background
- Loading progress + custom cursor
- Background music player and SFX
- Sakura / decorative particle scripts
- Share card and social links
- Responsive layout with themed CSS (`res/v5`)

## Stack

- HTML5 · CSS3 · vanilla JavaScript
- Remix Icon · jBox · local asset packs under `res/v5`

## Project layout

```
First/
├── index.html          # Entry
├── scripts/            # music, sakura, mouse, anti-inspect helpers
├── res/v5/             # themes, css, libs, media
├── *.mp3 / *.jpg       # tracks & art
└── LICENSE
```

## Run locally

```bash
git clone https://github.com/duckzangryy/personal-site-v1.git
cd First
# any static server
npx serve .
# or
python3 -m http.server 8080
```

Open `http://localhost:8080`.

## Customize

| Goal | Where |
|------|--------|
| Title / meta / OG | `index.html` `<head>` |
| Copy & sections | `index.html` body |
| Theme colors | `res/v5/css/*.css` |
| Music tracks | root `*.mp3` + `scripts/music.js` |
| Particles / effects | `scripts/sakura.js`, `scripts/cat.js`, … |

## Notes

- Some scripts intentionally discourage DevTools abuse (`no_dev.js`) — remove for clean forks.
- Large media files live in-repo; clone size is large.
- Prefer HTTPS in production for media autoplay policies.

## License

See [LICENSE](./LICENSE).
