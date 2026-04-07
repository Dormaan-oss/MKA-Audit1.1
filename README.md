# MKA Kurzaudit

Eine mobile Web-App für das mehrschichtige Kurzaudit. Läuft vollständig im Browser – **keine Internetverbindung erforderlich**, keine Installation, keine Server.

---

## Features

- **Zwei Auditprofile** – Mitarbeiter & Schichtführer, jeweils mit eigenem Fragenkatalog
- **Fragen verwalten** – Fragen hinzufügen, bearbeiten und löschen über die Einstellungen
- **Statusbewertung** – Jede Frage wird per Tipp bewertet: ✓ In Ordnung / ⚠ Auffällig / ✗ Mangelhaft
- **Kommentarfeld** – Pro Frage optional einen Kommentar eingeben
- **Ergebnisübersicht** – Zusammenfassung aller Bewertungen nach dem Audit
- **Excel-Export** – Tabellenansicht zum Kopieren und direkten Einfügen in Excel
  - Lange Kommentare (> 20 Zeichen) werden als „siehe Bemerkung" gekennzeichnet und am Ende gesammelt

---

## Verwendung

### Option 1 – Direkt im Browser öffnen (offline)
1. Datei `index.html` herunterladen
2. Auf dem Smartphone oder PC im Browser öffnen
3. Fertig – keine Internetverbindung nötig

### Option 2 – GitHub Pages (online erreichbar)
1. Repository auf GitHub erstellen
2. Unter **Settings → Pages** die Branch `main` und den Ordner `/root` auswählen
3. Die App ist dann unter `https://<dein-username>.github.io/<repo-name>/` erreichbar

### Option 3 – Als Android-App installieren (PWA)
1. `index.html` auf einem Webserver oder via GitHub Pages bereitstellen
2. Im Chrome-Browser auf Android die Seite öffnen
3. Über **Menü → Zum Startbildschirm hinzufügen** installieren
4. Die App erscheint wie eine native App auf dem Homescreen

---

## Excel-Export – Funktionsweise

Nach Abschluss eines Audits unter **„Tabelle für Excel anzeigen"**:

- Jedes Feld steht in einer eigenen Zeile (Nr., Frage, Status, Kommentar)
- Kommentare mit mehr als 20 Zeichen erscheinen als `siehe Bemerkung`
- Die vollständigen Kommentare werden am Ende gesammelt: `Bemerkungen: (1) Text... (3) Text...`
- Text markieren → kopieren → in Excel einfügen → jede Zeile landet in einer eigenen Zelle

---

## Technologie

- Reines HTML/CSS/JavaScript – eine einzelne Datei, keine Abhängigkeiten
- Kein Framework, kein Build-System, kein Backend
- Funktioniert auf Android, iOS, Windows, macOS

---

## Lizenz

Dieses Projekt ist für den internen Gebrauch bei MKA erstellt.
