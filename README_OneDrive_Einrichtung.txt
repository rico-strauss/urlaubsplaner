EINRICHTUNG: PRIVATER ONEDRIVE-SYNC

1. Microsoft Entra Admin Center öffnen und eine neue App registrieren.
2. Unterstützte Kontotypen: nur persönliche Microsoft-Konten oder persönliche plus Organisationskonten. Diese PWA verwendet die Authority 'consumers' und meldet damit private Microsoft-Konten an.
3. Unter Authentifizierung eine Plattform 'Single-Page-Anwendung' hinzufügen. Als Redirect-URI die exakte HTTPS-Adresse der Datei eintragen, z. B. https://example.github.io/urlaub/Urlaubsplaner_Private_OneDrive_PWA.html
4. Unter API-Berechtigungen delegiert hinzufügen: Microsoft Graph > Files.ReadWrite.AppFolder und User.Read. Kein Client-Secret anlegen oder in die PWA einbauen.
5. Die Anwendungs-ID (Client-ID) in config.js einsetzen.
6. Alle Dateien gemeinsam auf einem HTTPS-Webspace veröffentlichen. Danach die PWA öffnen und 'Mit Microsoft anmelden' wählen.

SPEICHERUNG
Die Daten liegen in OneDrive im geschützten App-Ordner unter Apps/<App-Name>/urlaubsplaner-private.json. Zusätzlich bleibt ein lokaler Offline-Stand im Browser. Bei erneutem Netz synchronisiert die App. Bei konkurrierenden Änderungen verhindert ETag/If-Match ein blindes Überschreiben und lädt den Cloud-Stand neu.

WICHTIG
Ein direktes Öffnen über file:// funktioniert nicht für OAuth/PWA. HTTPS oder localhost ist erforderlich. Der Client-ID-Platzhalter ist absichtlich nicht vorausgefüllt, weil jede private App-Registrierung eine eigene ID benötigt.
