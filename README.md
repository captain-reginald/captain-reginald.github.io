# captain-reginald.github.io

Two static sites served from this repo via GitHub Pages:

- `/` — landing page: a short intro, Rain Log, and Captain's Cabin (Minecraft)
- `/rainlog/` — the three Rain Log releases (Omarchy plugin, server, desktop app) and the shared data file

Plain HTML and CSS, one stylesheet, no build step, no JavaScript.

## Publishing

GitHub Pages serves `main` from the repo root. Push, and it is live:

- <https://captain-reginald.github.io/>
- <https://captain-reginald.github.io/rainlog/>

## Pending

**Discord invite link.** The landing page shows a "invite link coming soon" pill on purpose. When the invite is final, edit `index.html` (in the `#cabin` section; there is a `DISCORD-INVITE` comment) and replace the `<span class="soon">` with `<a href="https://discord.gg/…">Join the Discord</a>`. Access is gated by Discord's server verification, not by the page.

## Editing

- Shared styles: `/style.css` (design tokens at the top: background, text, accent, fonts).
- Screenshots live in `rainlog/assets/`, copied from the project repos. Keep the filenames in place; the HTML references them directly.
  - `plugin-*.png` from `omarchy-rain-log`
  - `server-*.png` from `rainlog-server/screenshots/`
  - `desktop-*.png` from `rainlog-desktop/docs/`
- `404.html` is served by Pages for unknown paths.
