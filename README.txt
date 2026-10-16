DadiCare — PWA package (Print Summary edition)

CONTENTS
- index.html: DadiCare dashboard with date-range Print Health Summary
- manifest.webmanifest: installable app metadata and unique app identity
- service-worker.js: offline app-shell caching
- icons/: install icons

PUBLISH WITH GITHUB PAGES
1. Create a separate public GitHub repository for this version (recommended to avoid mixing it with another dashboard/PWA).
2. Upload the CONTENTS of this folder to the repository root. Make sure index.html, manifest.webmanifest, and service-worker.js are at the root, not inside another folder.
3. In repository Settings > Pages, deploy from branch main and folder /(root). Save and wait for deployment to finish.
4. Open the resulting HTTPS GitHub Pages URL in Chrome on Android. Load it once while online.
5. Chrome menu (⋮) > Install app (or Add to Home screen, depending on Chrome's wording).

NOTES
- The dashboard keeps records in browser local storage. Existing data is available only when this page runs at the same origin/browser storage location as the previous version. Before replacing a live site, export a JSON backup from the dashboard.
- GitHub Pages repositories are public. Do not put private health records in repository files. The app's user-entered records remain in browser storage, but this is not a substitute for a secure medical-record system.
- The service worker enables the app shell to open offline after its first successful online visit; first-time installation requires internet.
