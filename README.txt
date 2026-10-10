STAFF ATTENDANCE PWA — OFFLINE UPDATE

This folder adds a web app manifest, service worker, and app icons to the existing Staff Attendance app. The original app features and localStorage key are retained.

IMPORTANT: Keep your current live app and JSON backup. Do not delete existing app data. Before deployment, export a JSON backup from Settings & Backup.

PUBLISHING TO GITHUB PAGES
1. Extract this ZIP on your Mac.
2. Open your Staff Attendance GitHub repository.
3. Upload/replace index.html and add manifest.json, service-worker.js, icon.svg, and apple-touch-icon.png to the SAME folder as index.html (usually the repository root).
4. Commit changes and wait for GitHub Pages to publish.
5. On iPhone, open the GitHub Pages URL while online and wait for the app to finish loading. Close it and reopen it once online so the service worker can install and cache files.
6. Test with Airplane Mode ON. Verify the app opens and attendance can be saved.

DATA SAFETY
Attendance records are stored in this browser's localStorage under staffAttendanceData_v1. This update does not move records between different URLs or devices. If the app's URL changes, restore a JSON backup only after exporting a fresh backup and checking the target app carefully.

Offline caching of app files does not itself guarantee that saved data is backed up. Export JSON backups regularly.
