DadiCare — PWA update (Print Summary edition)

This package is intended to UPDATE your existing DadiCare installation when deployed to the SAME GitHub Pages website URL. The app identity is kept stable. Do not create a second repository if you want the installed app to update in place.

UPLOAD
1. Download and extract this ZIP.
2. Open the SAME GitHub repository that currently hosts DadiCare.
3. Replace/update index.html, manifest.webmanifest, and service-worker.js; upload the icons/ folder too. Keep icons inside the icons folder.
4. Commit the changes and wait for GitHub Pages to finish deploying.
5. Open the existing DadiCare website in Chrome while online, refresh it, then close and reopen the installed DadiCare app. If it does not update, open the website again and wait a little for the service worker to update.

IMPORTANT
- The installed app is tied to its website URL. If you publish this package at a different URL, Chrome may treat it as a different app.
- Keep a JSON backup of existing records before replacing files. Records remain in browser storage only when the website origin and app code's storage key stay the same.
- GitHub Pages repository files are public. Do not upload private health records.
- For first-time setup, GitHub Pages must be deployed over HTTPS. The ZIP itself cannot be installed directly as an app.
