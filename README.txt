JAPAN 2027 TRAVEL COMPANION - PWA PACKAGE

WHAT THIS PACKAGE DOES
- Installable web app when hosted on HTTPS.
- Offline app shell and itinerary after the first successful online load.
- Editable itinerary, activities, bookings and notes.
- Google Maps links open when internet access is available.
- Local edits are saved in the current browser on the current device.
- JSON export/import is included for backup and manual transfer.

IMPORTANT ABOUT SYNC
This package does NOT yet provide automatic multi-device cloud sync. That requires a hosted backend/database and user authentication (for example, a Supabase project). No account credentials have been supplied, so no private cloud service has been connected. For now, use Toolkit > Export JSON Backup, save the JSON in iCloud Drive, and import it on another device. Avoid editing on two devices simultaneously before merging backups.

HOSTING REQUIREMENT
Service workers and PWA installation require HTTPS hosting (or localhost). Opening index.html directly from Files will not enable reliable offline caching or Add to Home Screen installation.

DEPLOY OPTION: GITHUB PAGES
1. Create/sign in to a GitHub account.
2. Create a new public repository, e.g. japan-2027-travel-companion.
3. Upload all files in this folder to the repository root: index.html, manifest.webmanifest, sw.js, icon-192.png, icon-512.png.
4. In repository Settings > Pages, choose Deploy from a branch, branch main, folder /(root), Save.
5. Wait for GitHub Pages to publish the HTTPS URL.
6. Open that URL in iPhone Safari while online.
7. Tap Share > Add to Home Screen > Add.
8. Open the new home-screen icon once while online. Then test Airplane Mode to verify cached itinerary availability.

MANUAL CROSS-DEVICE SYNC
1. In the app, open Toolkit and choose Export JSON Backup.
2. Save the JSON file to iCloud Drive.
3. On the other device, open the hosted app, go to Toolkit > Import backup, and select the JSON file.
4. Export a fresh backup after making changes. Treat the latest backup as the current master copy.

Google Maps links require connectivity. The itinerary itself is cached for offline use, but live maps, routing, traffic and map tiles are not guaranteed offline.
