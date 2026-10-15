# Doorframe

Track height, weight, birth details and milestones for your children. Installable on your phone, works offline, and keeps all data on the device.

## Files

```
index.html
manifest.webmanifest
sw.js
icons/icon-192.png
icons/icon-512.png
icons/icon-maskable-512.png
icons/apple-touch-icon.png
```

Keep the `icons` folder next to `index.html`.

## Put it on GitHub Pages

1. Create a new repository, for example `Doorframe`.
2. Upload all the files above, keeping the `icons` folder.
3. In the repository, go to Settings → Pages, set the source to the `main` branch and the root folder, then save.
4. After a minute it's live at `https://<your-username>.github.io/Doorframe/`.

## Install on a phone

- **iPhone (Safari):** open the link, tap Share, then Add to Home Screen.
- **Android (Chrome):** open the link and tap Install when prompted, or open Settings in the app and tap Install.

## Releasing an update

1. Replace `index.html` in the repository.
2. In `sw.js`, bump `VERSION` (for example `doorframe-v1.0.1`). In `index.html`, bump `APP_VERSION` to match.
3. Next time the app opens, it shows "A new version is ready". Tap Update.

If you skip step 2, phones keep using the cached copy.

## Data

- Everything is saved in the browser on that device. Nothing is sent anywhere.
- Each phone has its own copy. Use Settings → Save backup file, then Restore from file on the other phone to move data across.
- To bring data over from the Claude version: in that page, tap Copy backup, then in this app go to Settings → Paste a backup → Restore pasted backup.
