# UZH.ai Demo Gallery

Live, working AI demos built by [UZH.ai](https://www.uzh.ai/), the University of Zurich's AI initiative. Hosted via GitHub Pages: https://ai-uzh.github.io/uzh-ai-demos/

## Adding a new demo

No build step, no framework — just edit `index.html`.

The page has two sections, each backed by its own array inside the `<script>` tag near the bottom:

- **`demos`** — apps UZH.ai itself built. Renders under "Live demos".
- **`networkTools`** — apps built by researchers/collaborators in the UZH.ai network, not by UZH.ai. Renders under "From our network" with a distinct teal tag and a `credit` line.

To add an entry, copy an existing object in the relevant array and fill in:
- `tag` — `"Live demo"` for `demos`, `"From our network"` for `networkTools`
- `title` — the app's name
- `description` — one or two sentences on what it does
- `url` — the live (e.g. Vercel) URL
- `icon` — an inline SVG string (keep it simple/line-based, matching the existing icons)
- `credit` — (networkTools only) who built it, e.g. `"Built by a researcher in the UZH.ai network"`

Commit and push to `main` — GitHub Pages redeploys automatically within a minute or two. No other changes are needed; both grids render from these arrays automatically.
