# Game Night 🎲

A zero-build, mobile-friendly board game picker made from your BoardGameGeek collection export.

## Publish on GitHub Pages
1. Make a new public GitHub repository (e.g. `game-night`).
2. Upload `index.html` to the root of the repository (you can also upload `games.json` for reference).
3. Go to **Settings → Pages → Build and deployment**, select **Deploy from a branch**, choose **main** and **/(root)**, and save.
4. Open the GitHub Pages URL displayed there. No build tools, API keys, or server required.

## Important
- Your original **169 owned games** are embedded directly in `index.html`, so the page works on its own.
- The games you **add or edit are saved in localStorage**, which means they're **per browser/device**, not synchronized between phones and laptops or published for visitors. Export **Data → Export my library (JSON)** and re-import elsewhere to transfer them. For permanent changes for *all* visitors, update the embedded game data in `index.html` or re-generate that file with your latest data.
- Player and duration filters accept **overlapping ranges** by default; tick the stricter checkboxes to require support for every player count / entire duration within limits.
- Missing personal ratings are treated as *unrated*, not bad reviews. Missing complexity / BGG rating does not prevent a result unless you add a specific filter (missing values remain eligible).
- Time slider tops out at **180+ minutes**, player slider at **12+**; unusually large games can still show.
- There is no external JS dependency. A Google Fonts stylesheet is optional; the site still works offline with fallback fonts.
- JSON and CSV import **replace** your current library (you'll be asked to confirm), they do not merge.
