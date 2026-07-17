# Society That Learns — Webinar Page

`webinar-stl.html` is the bilingual (Thai/English) invite page for **The Society That Learns** book webinar (Wednesday 22 July 2026, 9:00 AM Thailand time, on Zoom) with Paulo Blikstein and Deborah A. Fields.

## Publishing setup (two repos)

- **Source of truth (this repo):** `society-that-learns-book/webinar-stl.html` in [arnans/paron-principle](https://github.com/arnans/paron-principle). Edit the page here.
- **Public site:** https://arnans.github.io/stl-webinar/ — served by GitHub Pages from a separate repo, [arnans/stl-webinar](https://github.com/arnans/stl-webinar), where the file is a copy renamed to `index.html`. A separate repo is used so the invite gets a short, clean URL.

The two copies do **not** sync automatically.

## How to update the live page

1. Edit `webinar-stl.html` here, then commit and push this repo.
2. Copy the file into the local clone of the site repo as `index.html`, e.g. from the root of this repo:
   ```
   copy society-that-learns-book\webinar-stl.html C:\Users\arnan.s\Documents\stl-webinar\index.html
   ```
3. Commit and push `stl-webinar`. GitHub Pages redeploys automatically within a minute or two.

## Notes

- The page is fully self-contained (images embedded as base64, inline SVG icons); only the Google Fonts (Sarabun / Noto Serif Thai) load from the network, with system fallbacks offline.
- The Zoom link, Meeting ID, QR code, and Google Calendar button all point to the same meeting — if the Zoom link ever changes, update all four.
