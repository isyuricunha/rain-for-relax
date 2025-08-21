# A Rain with Music to Relax

Rain for Relax is a minimal, single-page ambient app that plays rain sounds over a looping background video. It is designed to help you unwind, focus, or sleep with a distraction-free interface.

- Live site: https://www.rain-for-relax.yuricunha.com/
- Tech: Plain HTML + CSS, no build step, static assets only

---

## Features

- Simple, calming interface centered on a looping rain video (`assets/chill-rain.mp4`)
- Auto-loop rain audio (`assets/rain-chill.mp3`)
- One-click start link to comply with browser autoplay policies
- Lightweight: no frameworks, no client-side routing, no external state
- Social/contact links (GitHub, Discord, E-mail, Telegram, Website, LinkedIn)
- Deployed as static site (GitHub Pages or Vercel)

## How it works

The app is built from two files:

- `index.html` — The entire UI, including:
  - Background `<video id="background-video">` source at `assets/chill-rain.mp4`
  - `<audio autoplay loop>` source at `assets/rain-chill.mp3`
  - Centered content container `.centered` showing logo and links
  - A refresh link to prompt user gesture: `And, click here to begin.`
  - Analytics snippets: Google Analytics (gtag) and Umami
- `main.css` — Visual styling (fonts, layout, hover states, simple animations)

Supporting assets live under `assets/`:

- `assets/chill-rain.mp4` — background video (looped)
- `assets/rain-chill.mp3` — rain audio (looped)
- `assets/images/` — icons: `cloud.png`, `github.png`, `discord.png`, `mail.png`, `telegram.png`, `website.png`, `linkedin.png`, `logo.png`, `logo.ico`

Deployment and metadata:

- `.github/workflows/static.yml` — GitHub Pages deploy workflow
- `.github/workflows/auto-release.yml` — automated tagging and releases
- `vercel.json` — Vercel GitHub integration configuration
- `license.md` — custom personal license by the author

## Project structure

```
.
├─ index.html
├─ main.css
├─ assets/
│  ├─ chill-rain.mp4
│  ├─ rain-chill.mp3
│  └─ images/
│     ├─ cloud.png
│     ├─ github.png
│     ├─ discord.png
│     ├─ mail.png
│     ├─ telegram.png
│     ├─ website.png
│     ├─ linkedin.png
│     ├─ logo.png
│     └─ logo.ico
├─ .github/workflows/
│  ├─ static.yml
│  └─ auto-release.yml
├─ vercel.json
├─ license.md
└─ readme.md
```

## Local development

No build tools are required.

1. Clone the repo.
2. Open `index.html` directly in your browser, or serve the folder via any static server.
3. If your browser blocks autoplay audio, click the “click here to begin” link to start playback.

Tip: to run a simple server (examples):

- Python 3: `python -m http.server 8000`
- Node (serve): `npx serve .`

## Deployment

This is a static site; deploy any way you prefer. Two options are provided in-repo.

### GitHub Pages

- Workflow: `.github/workflows/static.yml` uploads the repository as a Pages artifact on pushes to `main`.
- Ensure Pages is enabled in the repository settings and points to GitHub Actions.

### Vercel

- You can import the repository into Vercel.
- `vercel.json` currently only silences GitHub comments, but default static deployment works.

## Customization

- Background video: replace `assets/chill-rain.mp4` and update `index.html` `<source>` if you change the filename.
- Audio loop: replace `assets/rain-chill.mp3` and update `index.html` `<source>` if you change the filename.
- Logo: update `assets/images/cloud.png` and `#logo` in `index.html`.
- Text copy: edit the heading and link text in `index.html`.
- Styles: tweak sizes, typography, and hover effects in `main.css`.
- Social links: update the `<a>` tags in `index.html`.

## Accessibility and UX notes

- Autoplay restrictions: Many browsers block autoplay with sound. The page includes a prominent link that triggers a navigation refresh, which counts as a user gesture and starts audio.
- Color/contrast: Text is white over a moving background. If needed, consider adding a semi-opaque overlay behind text for improved readability.
- Keyboard: Page has no interactive controls beyond links; tab order is minimal. Consider adding a play/pause control for audio for better accessibility.
- Motion: Background video is always on. Consider an optional “reduce motion” toggle for sensitive users.

## Privacy and analytics

This site includes:

- Google Analytics (gtag) with measurement ID `G-YMBMJST8GR`
- Umami analytics script from `https://umami.yuricunha.com/` with `data-website-id="ae078a6c-02fb-45c2-96d3-3274da991093"`

If you fork this project, replace or remove these analytics snippets in `index.html`.

## Troubleshooting

- No audio on load: Click the “click here to begin” link or interact with the page to satisfy autoplay policies.
- Video not loading: Confirm `assets/chill-rain.mp4` exists and the path in `index.html` matches.
- Broken icons: Check image filenames and paths in `assets/images/`.
- GitHub Pages not updating: Ensure Actions succeeded and Pages is set to deploy from GitHub Actions.

## Contributing

Contributions that improve accessibility, performance, or add optional controls (play/pause, volume, mute, reduce motion) are welcome.

1. Fork the repo
2. Create a feature branch
3. Make changes with clear commits
4. Open a pull request describing the change and rationale

For media contributions, ensure you have the rights to distribute the audio/video.

## License

This project is licensed under the author’s personal license. See `license.md` for details and terms on inspiration, attribution, and restrictions.

## Credits

- Author: Yuri Cunha
- Logo and icons: located under `assets/images/`
- Media: rain video and audio included under `assets/`

## Contact

Questions or feedback: me@yuricunha.com

---

Enjoy the rain and take a moment to breathe.
