KORRIGIERTE PWA V3

Redirect URI (SPA): https://rico-strauss.github.io/urlaubsplaner/
Client-ID: 0c69851d-0e41-457a-ad01-7966e0a05d68

Upload: index.html, config.js, manifest.webmanifest und sw.js im GitHub-Repository vollständig ersetzen. Danach GitHub Pages neu laden. Wegen Service-Worker-Cache auf allen Geräten die Seite einmal hart aktualisieren oder Website-Daten löschen.

Neu: explizite asynchrone MSAL-Initialisierung; handleRedirectPromise vor Login; Redirect-Anmeldung auf Smartphones; Popup auf Desktop mit Redirect-Fallback; sichtbarer Fehlercode und technische Details; direkter OneDrive-AppFolder-Sync.
