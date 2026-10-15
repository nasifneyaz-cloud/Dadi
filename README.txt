# DadiCare PWA

This folder is a ready-to-deploy Progressive Web App package.

## Included
- `index.html` — existing DadiCare dashboard and its existing features
- `manifest.webmanifest` — app name, icon, launch mode and theme
- `service-worker.js` — caches the app shell for offline reopening
- `icons/` — Android app icons

## Important: host over HTTPS
Android Chrome only offers PWA installation when the app is served from HTTPS (or localhost for testing). Opening `index.html` directly as a local file will not enable installation or offline service-worker caching.

## Deploy
Upload the *contents* of this folder to an HTTPS static host, keeping the folder structure. For example, use GitHub Pages or Netlify. Then open the deployed URL in Chrome on Android and choose `Install app` from the in-page button or Chrome's ⋮ menu.

## Data and privacy
DadiCare continues to use browser `localStorage` with the same key (`dadicare-v1`) and existing data format. Browser storage is tied to the site's origin. Data that was entered while opening the old `file://` HTML may not automatically appear after hosting the app at an HTTPS URL. Before switching, open the old dashboard and use Export CSV to back up readings; also keep the old file until you have checked the new hosted version. CSV export backs up readings, but does not export habit checkboxes.

The dashboard stores health information on the device/browser; this package does not send records to a server. Do not use a shared/public device, and keep a separate backup if the records matter.
