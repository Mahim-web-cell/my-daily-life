MY DAILY LIFE — iPhone starter PWA
===================================

Files
- index.html: task list, English/Bangla toggle, Quran reader and starter duas
- manifest.json: Home Screen app metadata
- sw.js: minimal service worker starter

IMPORTANT LIMITS
1. This is a starter web app, not a fully native iOS app.
2. Task reminders are scheduled in the page while it is open. iOS may suspend/stop the page when you leave it, so this version CANNOT guarantee alarms or repeat notifications while closed.
3. Reliable notifications while the app is closed require a secure hosted site, Home Screen installation, a push subscription, and a push server. The included service worker does not implement server push.
4. Quran text/translation/audio are fetched from Al Quran Cloud over the internet. This prototype uses quran-uthmani, bn.bengali, en.sahih and ar.alafasy editions. Confirm translation and recitation preferences before production.
5. Task data is stored in localStorage on this device/browser only; clearing website data can erase it. No cloud backup or sync.
6. Dua section is a small starter collection, not a complete verified daily-adhkar library.

HOW TO USE WITH ONLY AN IPHONE
A. Easiest route: use an online code editor/hosting service in Safari that lets you create and publish static files. Create a project and add these three files, then publish it to an HTTPS URL.
B. Open the published URL in Safari on the iPhone.
C. Tap Share -> Add to Home Screen -> enable Open as Web App (if shown) -> Add.
D. Open the new Home Screen icon, select English/Bangla, and test the Quran reader while online.
E. In Tasks, add a task with date/time. For this prototype, keep the app open to receive the in-page reminder. Tap Enable notifications if supported and grant permission.

Do not paste private passwords or API secrets into public code. This prototype needs no API key.
