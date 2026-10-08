# OOSH Attendance

Private attendance tracker for the OOSH after-school programme: daily check-in/out, picked-up flags,
weekly and monthly summaries, CSV exports. A single `index.html` PWA (offline shell via `sw.js`).

- **Live:** https://ooshonline.github.io/oosh-attendance/ (GitHub Pages, `main` branch, root)
- **Data:** Firebase project `oosh-attendance` (Firestore + email/password sign-in). Children's names
  and attendance live in Firestore behind sign-in, never in this repo. `localStorage` holds an offline
  copy on each device.
- **Deploy:** commit and push `main`; Pages publishes in about a minute. Bump `CACHE` in `sw.js` when
  `index.html` changes so installed copies refresh.
- **Outstanding:** publish `firestore.rules` in the Firebase console (Firestore → Rules).

Until 2026-10 this app lived inside the Ribbit Reading App repo at
`ooshonline.github.io/Oosh-online/oosh-attendance/`. That address now redirects here.
Development notes are kept locally in `dev-log.md` (not committed).
