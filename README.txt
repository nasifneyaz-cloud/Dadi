DadiCare — Updated PWA (same supplied logo)

This ZIP keeps the existing root-level logo/icon files 1.png, 2.png and 3.png and preserves the localStorage key dadicare_final_v2 so existing records in the same browser origin are not intentionally reset.

UPLOAD TO YOUR EXISTING GITHUB PAGES REPOSITORY
1. Download and extract this ZIP.
2. Open the existing repository: nasifneyaz-cloud/Dadi, branch main.
3. Upload/replace all seven files in the repository root: index.html, manifest.webmanifest, service-worker.js, 1.png, 2.png, 3.png, README.txt. Keep the filenames exactly as shown.
4. Commit the changes. Do not create a new repository or change the GitHub Pages URL.
5. Wait for Pages to deploy, then open https://nasifneyaz-cloud.github.io/Dadi/ in Chrome.
6. If the app was previously opened, close its tabs and reload the website. In Chrome, open the menu and check Install app / Add to Home screen.

IMPORTANT
- The ZIP fixes the manifest/icon paths and service-worker cache version. It cannot force Chrome to show Install app if the GitHub Pages deployment is not served over HTTPS, deployment has not finished, or Chrome still has stale site state.
- The existing icon images are included unchanged; no new logo was generated.
- Keep all files in the repository root, not inside a folder.
