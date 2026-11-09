# PG Manager

A simple mobile app for PG (paying guest) owners to track students, rent and electricity bills.
It is a Progressive Web App (PWA) that runs fully offline. There is no server, no login and no database. All data stays on the owner's phone.

## Features

- **Student database:** name, room number, phone, email and monthly rent, with search
- **Rent tracking:** see who is Pending or Paid this month, with a total of the pending amount
- **Safe Paid button:** a confirmation screen shows rent, electricity and total. The amount received must match before the tenant is marked **Cleared**. Undo is available.
- **Electricity billing:** enter the current meter reading. The bill is calculated automatically from the previous reading and the per-unit rate.
- **WhatsApp reminders:** one tap opens WhatsApp with a ready message (name, room, rent, electricity and total). The owner presses Send.
- **Backup:** Export all data to a JSON file and Import it back
- **Offline:** a service worker caches the app so it opens without internet
- Large buttons designed for one-handed use on a phone

## Files

| File | Purpose |
|------|---------|
| `index.html` | The whole app (HTML, CSS and JavaScript) |
| `manifest.json` | PWA details (name, colours, icons) |
| `sw.js` | Service worker for offline use |
| `icon-192.png`, `icon-512.png` | App icons |

## How to use

1. Host the files on GitHub Pages, Netlify or any HTTPS host (service workers need HTTPS).
2. Open the link in Chrome on Android and tap **Add to Home screen**.
3. Open **Settings** to set the PG name, owner name and electricity rate per unit.

## Make an Android APK

Paste your hosted link into [PWABuilder](https://www.pwabuilder.com) and choose Android.

## Data and backup

Data is stored in the browser's localStorage on one device. Clearing browser data or changing phones deletes it, so use **Settings → Export** regularly and keep the file safe.

## Tech

Plain HTML, CSS and JavaScript. No frameworks and no build step.
