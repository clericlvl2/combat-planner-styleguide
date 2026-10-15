# Combat Planner · Styleguide (dist)

Static build of the styleguide: every page, the sidebar and the runtime. No build step.

## Run locally
- macOS: double-click `start-mac.command` (first time: right-click → Open, or run `chmod +x start-mac.command`).
- Windows: double-click `start-windows.bat`.
- Any OS: `npx serve .` or `python3 -m http.server 8080` in this folder, then open http://localhost:8080/Styleguide.dc.html.

Opening the files straight from disk (file://) does not work: pages load each other over HTTP.

## Publish
Upload the folder as-is to any static host: Netlify Drop, Vercel, GitHub Pages, Cloudflare Pages, S3. `index.html` opens the styleguide.

## Notes
- Fonts (Unbounded, Rubik, Noto Sans JP) and icons (Tabler Icons 3.19) load from Google Fonts and jsDelivr, so an internet connection is needed for them.
- Pages: Styleguide.dc.html (entry, sidebar from nav.js) · Design: Tokens, Template, Baselines, Flow · Atoms, Molecules, Organisms · Pages: CombatScreen, PlayerView, CombatList, Library, AppPages. Screen pages accept `?flow=CODE`, e.g. CombatScreen.dc.html?flow=CS-F3.
