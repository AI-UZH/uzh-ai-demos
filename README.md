# UZH.ai Demo Gallery

Live, working AI demos built by [UZH.ai](https://www.uzh.ai/), the University of Zurich's AI initiative. Hosted via GitHub Pages: https://ai-uzh.github.io/uzh-ai-demos/

## Adding a new demo

No build step, no framework — just edit `index.html`.

1. Open `index.html` and find the `const demos = [ ... ]` array near the bottom (inside the `<script>` tag).
2. Copy one of the existing objects and add a new entry with:
   - `tag` — usually `"Live demo"`
   - `title` — the app's name
   - `description` — one or two sentences on what it does
   - `url` — the live (e.g. Vercel) URL
   - `icon` — an inline SVG string (keep it simple/line-based, matching the existing icons)
3. Commit and push to `main`. GitHub Pages redeploys automatically within a minute or two.

No other changes are needed — the card grid renders from that array automatically.
