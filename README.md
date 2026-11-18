# captain-reginald.github.io

The two static sites served from this repo, via GitHub Pages:

- `/` — the landing page: a short blurb, the Rain Log project, and Captain's Cabin (Minecraft)
- `/rainlog/` — overview of the three Rain Log releases (Omarchy plugin, server, desktop app) and how they share one data file

Plain HTML and CSS. No build step, no dependencies, no JavaScript.

## Publishing

GitHub Pages serves the default branch from the repo root. Push to `main` and it is live:

- <https://captain-reginald.github.io/>
- <https://captain-reginald.github.io/rainlog/>

## Pending

- **Discord invite link** — the landing page shows "invite link coming soon" as a placeholder on purpose. When the invite is final, edit `index.html` (the `#cabin` section, look for the `DISCORD-INVITE` comment) and swap the `<span class="pill">` for `<a href="https://discord.gg/…">Join the Discord</a>`. Discord's server verification handles gating; the page does not.

## Editing

- Screenshots live in `rainlog/assets/` and were copied from the project repos (`rainlog-server/screenshots/`, `rainlog-desktop/docs/`, and `omarchy-rain-log`). If the apps change visually, re-copy and keep the filenames so the HTML doesn't need to change.
- Both pages share the same design tokens (`--bg`, `--accent`, fonts) at the top of `style.css` and `rainlog/style.css` — update them in both places.
