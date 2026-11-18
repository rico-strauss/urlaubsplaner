PWA V3.2 - SILENT AUTO-LOGIN

Neu:
- Beim Start wird ein bereits im MSAL-localStorage bekanntes Microsoft-Konto automatisch erkannt.
- acquireTokenSilent() wird vor der OneDrive-Synchronisierung ausgeführt.
- Bei gültiger/erneuerbarer Sitzung startet OneDrive-Sync ohne Klick.
- Nur bei interaction_required/login_required/consent_required erscheint „Microsoft-Anmeldung erforderlich“.
- Lokaler Planer bleibt bei abgelaufener Sitzung nutzbar.

GitHub: index.html und sw.js ersetzen; config.js und manifest.webmanifest können unverändert mit hochgeladen werden. Danach GitHub Pages Deployment abwarten und einmal Strg+F5 bzw. PWA neu starten.
