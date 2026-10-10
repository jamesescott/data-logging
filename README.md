# Data Logging

A private, offline-capable static web app for logging numeric measurements on Android and desktop browsers.

## Deploy to GitHub Pages

Upload `index.html`, `app.js`, `style.css`, `manifest.json`, `service-worker.js`, and `icon.svg` to the repository root. In **Settings → Pages**, select **Deploy from a branch**, `main`, `/ (root)`.

## Features

- Multiple logs with names, descriptions and units
- Numeric entries with automatic or user-specified date/time
- Chart with selectable time range
- CSV import/export (`date,value`), including date-only historical values
- Duplicate prevention on CSV import by date and value
- JSON backup and restore of all logs
- IndexedDB local storage, installable PWA, offline caching

## Privacy and backup

Records stay in the browser's local IndexedDB, not on GitHub. Each device maintains a separate database. Export JSON backups regularly; clearing browser site data can erase logs. CSV files do not include log metadata. There is no automatic cross-device sync.
