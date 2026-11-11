TABLET TURN READER — INSTALLABLE OFFLINE WEBSITE

This folder is an optional PWA (progressive web app) version of the single-file Tablet Turn Reader.

1. Unzip all files into the same folder on a web server.
2. Publish the folder over HTTPS (necessary for iOS offline caching / PWA installation).
3. Open the index.html URL in Safari on your iPhone.
4. Tap Share > Add to Home Screen, then open the new home-screen app while online.
5. After the files have cached, the app can reopen and operate without network access.

The pattern and selected pick are saved locally in the same browser/app storage.

Running index.html on a plain HTTP server on the home LAN is fine for normal online use but generally does not allow the offline service worker on iOS.

Do not open HTML through the iOS Files/Quick Look preview: that can display the page but block its buttons/scripts.

FILES: index.html, sw.js, manifest.webmanifest, icon-192.png, icon-512.png.

The dark mode preference is saved on this device, alongside the weaving pattern and current pick.

Version 7: dark mode and pattern buttons aligned in the header; collapsible full pattern overview.
