# West Yorkshire Demographic Evidence Dashboard

A self-contained interactive dashboard. One HTML file, no build step, nothing to install.
D3.js is already embedded, so it works offline and on any static host.

## Files
- `index.html` - the whole dashboard. Double-click to open it in a browser.

## Host it free on GitHub Pages (gives a URL with no "claude" in it)
1. Create a free GitHub account if you do not have one.
2. Create a new PUBLIC repository, for example `wy-demographics`.
3. Add `index.html` to it (drag-and-drop on github.com, or push from VS Code).
4. In the repo: Settings > Pages.
5. Build and deployment: Source = "Deploy from a branch"; Branch = `main`; Folder = `/ (root)`. Save.
6. Wait 1-2 minutes. Your live URL will be:
   `https://<your-username>.github.io/wy-demographics/`
   Share that link in the slide and with the panel.

## Use it in VS Code
1. Open the folder in VS Code.
2. Install the "Live Server" extension, then right-click `index.html` > "Open with Live Server" to preview.
3. Commit and push from the Source Control panel to update the live site.

## Editing the content
Everything lives in `index.html`, inside the `<script>` tag near the bottom:
- `DATA` - the district figures
- `INDICATORS` - the six data views and their captions
- `TYPO` / `CATS` - the Implications typology (analyst interpretation)
Change the values and refresh the page.

## Data and credits
Built with HTML, CSS, JavaScript and D3.js v7 (embedded).
Data: ONS mid-2021 local authority population estimates; household change from
Census 2011 and Census 2021. Boundaries: ONS Open Geography (Local Authority Districts).
The Implications view is analyst interpretation of that data, not an ONS dataset.
