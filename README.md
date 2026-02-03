# Rebeccapedia

Lokales Tool zur Erstellung von Übungsmaterialien für Klassen 1–10 (Mathe, Deutsch, Englisch).

## Start

1. Ordner im Finder öffnen
2. `index.html` doppelklicken (öffnet im Browser)
3. Fertig - keine Installation notwendig

**Hinweis:** Funktioniert komplett offline. Alle Daten bleiben lokal im Browser.

---

## PWA / Mobile-Installation

### iPhone/iPad (Safari):
1. Öffne https://rebeccapedia.pages.dev in Safari
2. Tippe auf das „Teilen"-Symbol (□↑)
3. Wähle „Zum Home-Bildschirm"
4. Die App ist jetzt wie eine native App nutzbar (offline-fähig)

### Android (Chrome):
1. Öffne https://rebeccapedia.pages.dev in Chrome
2. Tippe auf die drei Punkte (⋮)
3. Wähle „App installieren" oder „Zum Startbildschirm hinzufügen"
4. Die App startet als eigenständige Anwendung

### Desktop (Chrome/Edge):
1. Öffne https://rebeccapedia.pages.dev
2. Klicke auf das ⊕-Symbol in der Adressleiste
3. Oder: Menü → „Rebeccapedia installieren"

**Offline-Nutzung:** Nach der Installation funktioniert die App auch ohne Internet.

---

## Demo-Flow in 6 Schritten

### 1. Klassenstufe wählen
Wähle eine Klasse von **1 bis 10**

### 2. Fach wählen
Klicke auf eine Kachel: **Mathe**, **Deutsch** oder **Englisch**
(Verfügbarkeit je nach Klasse)

### 3. Thema wählen
Wähle eines der verfügbaren Unterthemen (z.B. "Addition & Subtraktion bis 1000" für Klasse 3)

### 4. Einstellungen anpassen
- Schwierigkeitsstufe (Level 1-3 oder einzeln)
- Anzahl Aufgaben pro Level
- Mini-Test ja/nein
- Sprachstil

### 5. Prompt kopieren & in ChatGPT/Claude einfügen
- Klicke „Prompt kopieren"
- Öffne ChatGPT oder Claude
- Füge den Prompt ein und sende ihn
- Kopiere die JSON-Antwort

### 6. JSON importieren & nutzen
- Füge die JSON-Antwort in das Textfeld ein
- Klicke „Importieren"
- Arbeitsblatt wird gerendert
- **NEU:** Wähle zwischen:
  - **📄 PDF drucken** → Saubere Print-Ansicht (A4, nichts abgeschnitten)
  - **✏️ Online-Übungsblatt** → Interaktiv im Browser ausfüllen + Prüfen

---

## Online-Übungsblatt (Neu!)

Das **Online-Übungsblatt** ermöglicht interaktives Arbeiten:

✅ **Mathe-Aufgaben automatisch prüfen**
- Eingabe der Antwort
- Sofortiges Feedback (✓ Richtig / ✗ Noch mal)
- Nach 2 Fehlversuchen: Tipp anzeigen
- Nach 3 Versuchen: Lösung zeigen

✅ **Auto-Save**
- Alle Eingaben werden automatisch gespeichert (localStorage)
- Beim erneuten Öffnen sind die Antworten wiederhergestellt

✅ **Bulk-Aktionen**
- „✓ Alle prüfen" – Prüft alle ausgefüllten Aufgaben auf einmal
- „↺ Zurücksetzen" – Löscht alle Eingaben

---

## PDF/Print-Optimierung (Neu!)

Die **dedizierte Print-Ansicht** (Button "📄 PDF drucken") bietet:

✅ **Perfekt für A4-Druck**
- Optimierte Ränder (12mm)
- Keine abgeschnittenen Umrandungen
- Modernes, schlichtes Layout

✅ **Gut beschreibbar**
- Kopfzeile mit Name/Datum-Linien zum Ausfüllen
- Antwortlinien unter jeder Aufgabe
- Optional: Rechenweg-Block für Mathe

✅ **Professionell**
- Saubere Schrift (11pt)
- Optimale Abstände
- Pagebreaks an den richtigen Stellen

**Tipp:** Im Print-Dialog "Als PDF speichern" wählen für digitale Archivierung.

---

## Datenschutz-Hinweis

**Keine personenbezogenen Daten eingeben!**

- Keine Schülernamen
- Keine Noten
- Keine Förderpläne
- Keine identifizierenden Informationen

Die App speichert nur lokal im Browser (localStorage). Keine Server-Uploads.

---

## Tipps

### JSON passt nicht?
Wenn ChatGPT/Claude kein sauberes JSON liefert:
1. Schreibe in deiner Nachricht: *"Bitte antworte nur mit dem JSON, kein Text davor oder danach."*
2. Oder: *"Gib das JSON ohne Markdown-Codeblock aus."*

### Markdown-Codeblock?
Die App erkennt JSON auch innerhalb von \`\`\`json ... \`\`\` Blöcken automatisch.

### Validation schlägt fehl?
Prüfe die Fehlermeldung - sie zeigt genau, welches Feld fehlt.

### Legacy-Hinweis?
Alte JSONs mit `"tool": "Rebeccademie"` werden weiterhin unterstützt.
Für neue Arbeitsblätter bitte `"tool": "Rebeccapedia"` verwenden.

---

## Struktur

```
rebeccapedia/
├── index.html           # Hauptdatei (HTML + CSS + JS inline)
├── topic-packs.json     # Themen-Datenbank (Klassen 1-10)
├── manifest.webmanifest # PWA Manifest
├── sw.js                # Service Worker (offline cache)
└── README.md            # Diese Datei
```

---

## Fächer & Themen (Auswahl)

### Klasse 3 (vollständig)
**Mathe**
- M31: Addition/Subtraktion bis 1000
- M32: Einmaleins & Division
- M33: Sachaufgaben
- M34: Größen & Einheiten
- M35: Geometrie Grundlagen

**Deutsch**
- D31: Wortarten erkennen
- D32: Groß-/Kleinschreibung
- D33: Satzzeichen
- D34: Leseverstehen
- D35: Bildergeschichte schreiben

**Englisch**
- E31: Vocabulary (school/family/animals)
- E32: Satzmuster (I like/have/can)
- E33: Questions
- E34: Mini-Reading
- E35: Mini-Writing

### Klasse 5 (Beispiele)
**Mathe**
- M51: Bruchrechnung Grundlagen
- M52: Dezimalzahlen
- M53: Größen umrechnen

**Deutsch**
- D51: Zeitformen
- D52: Wortfamilien

**Englisch**
- E51: Simple Present & Present Progressive

### Weitere Klassen (1, 2, 4, 6–10)
Minimal-Themen verfügbar. Weitere Inhalte können über die Prompt-Funktion generiert werden.

---

## Technische Details

- **Framework:** Reine HTML/CSS/JS (keine Abhängigkeiten)
- **Offline:** PWA mit Service Worker (funktioniert auch ohne Internet)
- **Print:** Optimiertes CSS für A4-Druck (keine abgeschnittenen Ränder)
- **Mobile:** Touch-optimiert, responsive Design
- **Datenschutz:** Keine Telemetrie, keine Analytics, alles lokal
- **Deployment:** Cloudflare Pages (https://rebeccapedia.pages.dev)

### Browser-Kompatibilität
- ✅ Chrome/Edge (Desktop + Mobile)
- ✅ Safari (macOS + iOS)
- ✅ Firefox
- ⚠️ IE11 nicht unterstützt

---

## Entwicklung

### Lokaler Test
```bash
# Einfach index.html öffnen, oder:
python3 -m http.server 8000
# Dann: http://localhost:8000
```

### Service Worker testen
Service Worker funktioniert nur über HTTPS oder localhost.
Für lokale Tests: http://localhost:8000 verwenden.

---

## Lizenz

Frei zur Nutzung für Bildungszwecke.
