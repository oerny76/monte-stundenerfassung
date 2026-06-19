# 🌱 Familienarbeitsstunden Montessori-Campus Wertingen

Eine kleine, lokale Web-App zur Erfassung von Familienarbeitsstunden — installierbar als PWA auf iOS und Android, ganz ohne Server, ohne Account und ohne Cloud.

## Über das Projekt

Diese App wurde von **Ernest Jennen**, Elternteil am Montessori-Campus Wertingen, in Eigeninitiative entwickelt. Sie soll Familien dabei unterstützen, ihre geleisteten Arbeitsstunden unkompliziert auf dem eigenen Handy zu erfassen — und am Ende des Schuljahres (oder bei Bedarf) als CSV-Datei zu exportieren.

Die App ist **kein offizielles Werkzeug der Schule**, sondern eine freiwillige, private Unterstützung. Den vollständigen Haftungsausschluss findest du direkt in der App unter ⚙️ Einstellungen.

## Funktionen

- ➕ **Erfassen** – Datum, Dauer und Beschreibung eintragen, Kategorie optional auswählen
- 📋 **Verlauf** – alle Einträge einsehen, bearbeiten, einzeln oder im Batch löschen
- 📤 **Export** – als CSV herunterladen oder per E-Mail versenden
- 💾 **Backup** – vollständige Datensicherung als JSON-Datei, jederzeit wiederherstellbar
- ❓ **Hilfe** – integrierte Anleitung direkt in der App
- 📱 **PWA** – auf dem Homescreen installierbar, läuft offline

## Wie die App Daten speichert

Alle Einträge werden **ausschließlich lokal auf dem jeweiligen Gerät** im Browserspeicher (`localStorage`) abgelegt. Es gibt:

- keinen Server
- keine Cloud-Synchronisierung
- keinen Account / kein Login
- keine Übertragung von Daten an Dritte

Das bedeutet auch: Jede Person erfasst ihre Stunden auf ihrem eigenen Gerät. Mehrere Familienmitglieder (z. B. Vater und Mutter) nutzen die App unabhängig voneinander und führen ihre Daten am Ende über den CSV-Export zusammen.

⚠️ **Wichtig:** Da die Daten lokal im Browser liegen, können sie beim Leeren des Caches oder bei einer Neuinstallation des Browsers verloren gehen. Es wird empfohlen, regelmäßig ein JSON-Backup zu speichern (siehe Export-Tab).

## Installation auf dem Handy

1. Die App-URL im Browser öffnen (Safari auf iOS, Chrome auf Android)
2. **iOS:** Teilen-Symbol → „Zum Home-Bildschirm"
3. **Android:** Menü (⋮) → „Zum Startbildschirm hinzufügen" bzw. „App installieren"
4. Die App erscheint danach wie eine normale App auf dem Homescreen

## Lokales Hosting (GitHub Pages)

Dieses Repository enthält:

```
arbeitsstunden.html   ← Hauptanwendung
manifest.json         ← PWA-Manifest
icon-192.png          ← App-Icon (klein)
icon-512.png          ← App-Icon (groß)
```

Um die App über GitHub Pages bereitzustellen:

1. Repository-Einstellungen → **Pages** → Branch auswählen (z. B. `main`)
2. Die App ist anschließend erreichbar unter:
   `https://<benutzername>.github.io/<repo-name>/arbeitsstunden.html`

## Technologie

- Reines HTML/CSS/JavaScript — keine Build-Tools, keine Frameworks
- `localStorage` für die Datenhaltung
- Web Manifest für PWA-Installierbarkeit
- Keine externen Abhängigkeiten außer Google Fonts (DM Sans, DM Mono)

## Haftungsausschluss

Diese App wurde in Eigeninitiative ohne offizielle Beauftragung durch die Schule entwickelt. Sie erhebt keinen Anspruch auf Vollständigkeit, Richtigkeit oder rechtliche Verbindlichkeit. Für die Korrektheit der erfassten Stunden ist jede Familie selbst verantwortlich; die offiziellen Vorgaben der Schule sind maßgeblich. Der Entwickler übernimmt keine Haftung für Datenverlust oder Schäden durch die Nutzung dieser App.

## Lizenz / Nutzung

Frei nutzbar für Familien am Montessori-Campus Wertingen. Bei Fragen oder Verbesserungsvorschlägen gerne ein Issue eröffnen.

---

**Version 1.3.0** · Entwickelt von Ernest Jennen
