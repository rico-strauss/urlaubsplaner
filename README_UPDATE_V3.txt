KORRIGIERTE PWA V3

Redirect URI (SPA): https://rico-strauss.github.io/urlaubsplaner/
Client-ID: 0c69851d-0e41-457a-ad01-7966e0a05d68

Upload: index.html, config.js, manifest.webmanifest und sw.js im GitHub-Repository vollständig ersetzen. Danach GitHub Pages neu laden. Wegen Service-Worker-Cache auf allen Geräten die Seite einmal hart aktualisieren oder Website-Daten löschen.

Neu: explizite asynchrone MSAL-Initialisierung; handleRedirectPromise vor Login; Redirect-Anmeldung auf Smartphones; Popup auf Desktop mit Redirect-Fallback; sichtbarer Fehlercode und technische Details; direkter OneDrive-AppFolder-Sync.

KORREKTUR 18.11.2026: MSAL Browser wird als CDN-kompatible Version 2.35.0 geladen. MSAL Browser v3+ wird laut Microsoft nicht mehr auf diesem CDN bereitgestellt.
