# DAYMARK — Personal Performance Terminal

An iPhone-first, installable Progressive Web App (PWA) for tracking habits, weekly execution, and daily reflections. The design uses a dense, dark financial-terminal dashboard aesthetic with amber highlights and green completion states.

## Features
- Daily habit check-ins and completion percentage
- Weekly overview and weekly execution KPIs
- Add, edit, categorise, and delete habits
- Daily reflection notes
- Local-only persistence using browser localStorage
- JSON export and restore for backups
- Offline app shell via service worker
- Installable from Safari on iPhone after HTTPS hosting

## Deploy
1. Upload the contents of this folder to the root of a static HTTPS host (for example, GitHub Pages).
2. Open the hosted URL in Safari on iPhone.
3. Tap Share → Add to Home Screen. If offered, enable Open as Web App.

## Privacy and data
No account or cloud service is used. Habit data stays in the browser storage for that origin on that device. Export a JSON backup periodically; browser storage is not a substitute for a backup. Data does not automatically transfer between devices.

## Important
When updating an already-hosted installation, the service worker cache version is `daymark-terminal-v2`. Bump `CACHE_NAME` in `sw.js` when making future changes so devices fetch the new app shell.
