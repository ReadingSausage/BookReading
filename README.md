# Folio — Reading Tracker PWA

## Install on Android (Chrome)

1. **Host the files** — upload the entire folder to any static host:
   - **Netlify**: drag the folder onto netlify.com/drop — free, instant, HTTPS
   - **GitHub Pages**: push to a repo, enable Pages in Settings
   - **Vercel**: `npx vercel` in the folder

2. **Open in Chrome on Android** — navigate to your hosted URL

3. **Install prompt** — Chrome shows "Add to Home screen" banner automatically,
   or tap the three-dot menu → "Add to Home screen"

4. **Done** — Folio appears as a full-screen app with its own icon. Works offline.

## Files

```
folio-pwa/
├── index.html      Main app
├── manifest.json   PWA metadata + icons
├── sw.js           Service worker (offline caching)
├── icon-192.svg    Home screen icon
├── icon-512.svg    Splash screen icon
└── README.md       This file
```

## Data

All books and notes are stored in your browser's localStorage — they persist
between sessions and survive the app being closed. Clearing site data in Chrome
settings will reset to the default library.

## Notes system

- Click any book to open its detail panel
- Scroll to the Notes section (collapsible)
- Add a note with page number, text, tags (#quote #idea #question #important),
  and optional star
- Sort by: page number | comment length | starred first
- Toggle sort direction with ↑↓
- Star/unstar notes without reopening the form
- Delete notes (desktop: hover → ✕ appears; mobile: ✕ always visible)
