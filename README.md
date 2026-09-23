# Karobar — Universal Offline-First Business App

Karobar V1 is a browser-based Progressive Web App (PWA) for small shops, stalls and home businesses.

## Files

- `index.html` — main app
- `manifest.json` — PWA manifest
- `sw.js` — offline app-shell cache
- `css/style.css` — responsive UI
- `js/db.js` — IndexedDB database
- `js/app.js` — app/navigation/forms
- `js/inventory.js` — stock/items
- `js/sales.js` — sales/cart
- `js/purchases.js` — purchases
- `js/returns.js` — returns
- `js/customers.js` — customers/Udhaar
- `js/expenses.js` — expenses
- `js/reports.js` — reports/closing
- `js/backup.js` — JSON backup/restore
- `js/settings.js` — PIN
- `js/ui.js` — shared UI helpers

## Chromebook par chalana

1. ZIP extract karo.
2. Project ko kisi local web server ya static HTTPS host par open karo.
3. Browser mein `index.html` open karo.
4. Pehli dafa "Shuru Karein" dabao.
5. PWA install option browser support kare to install kar sakte ho.

Service Worker/PWA features `file://` se nahi chal sakte; localhost ya HTTPS use karo.

Agar Chromebook mein Linux available hai, project folder ke andar:
`python3 -m http.server 8080`
phir browser mein:
`http://localhost:8080`

## Important

- Data IndexedDB mein isi browser/device par save hota hai.
- V1 mein automatic cloud sync nahi hai.
- Doosre device par transfer ke liye Settings > Backup, phir doosre device par Restore.
- Currency PKR / Rs hai.
- UI Roman Urdu friendly hai.
- Core records ke liye third-party backend, Firebase, login ya analytics use nahi kiye gaye.

## Future APK

Is web app ko baad mein Capacitor jaisi wrapper technology se Android APK/AAB ke liye package kiya ja sakta hai. Current V1 ko browser/PWA ke taur par chalane ke liye Android Studio/Flutter required nahi.
