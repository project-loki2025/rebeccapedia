# Rebeccademie

Lokales Demo-Tool zur Erstellung von Ubungsmaterialien fur Grundschule Klasse 3.

## Start

1. Ordner in Finder offnen
2. `index.html` doppelklicken (offnet im Browser)
3. Fertig - keine Installation notwendig

**Hinweis:** Funktioniert komplett offline. Alle Daten bleiben lokal.

---

## Demo-Flow in 5 Schritten

### 1. Fach wahlen
Klicke auf eine Kachel: **Mathe**, **Deutsch** oder **Englisch**

### 2. Thema wahlen
Wahle eines der 5 Unterthemen (z.B. "Addition & Subtraktion bis 1000")

### 3. Einstellungen anpassen
- Schwierigkeitsstufe (Level 1-3 oder einzeln)
- Anzahl Aufgaben pro Level
- Mini-Test ja/nein
- Sprachstil

### 4. Prompt kopieren & in ChatGPT/Claude einfugen
- Klicke "Prompt kopieren"
- Offne ChatGPT oder Claude
- Fuge den Prompt ein und sende ihn
- Kopiere die JSON-Antwort

### 5. JSON importieren & drucken
- Fuge die JSON-Antwort in das Textfeld ein
- Klicke "Importieren"
- Arbeitsblatt wird gerendert
- Klicke "Drucken / PDF" fur den Export

---

## Datenschutz-Hinweis

**Keine personenbezogenen Daten eingeben!**

- Keine Schulernamen
- Keine Noten
- Keine Forderplane
- Keine identifizierenden Informationen

Die App speichert nichts. Alle Daten bleiben im Browser.

---

## Tipps

### JSON passt nicht?
Wenn ChatGPT/Claude kein sauberes JSON liefert:
1. Schreibe in deiner Nachricht: *"Bitte antworte nur mit dem JSON, kein Text davor oder danach."*
2. Oder: *"Gib das JSON ohne Markdown-Codeblock aus."*

### Markdown-Codeblock?
Die App erkennt JSON auch innerhalb von \`\`\`json ... \`\`\` Blocken automatisch.

### Validation schlagt fehl?
Prufe die Fehlermeldung - sie zeigt genau, welches Feld fehlt.

---

## Struktur

```
Rebeccademie/
├── index.html        # Hauptdatei (alles inline)
├── topic-packs.json  # Themen-Datenbank
└── README.md         # Diese Datei
```

---

## Facher & Themen

### Mathe
- M31: Addition/Subtraktion bis 1000
- M32: Einmaleins & Division
- M33: Sachaufgaben
- M34: Grossen & Einheiten
- M35: Geometrie Grundlagen

### Deutsch
- D31: Wortarten erkennen
- D32: Gross-/Kleinschreibung
- D33: Satzzeichen
- D34: Leseverstehen
- D35: Bildergeschichte schreiben

### Englisch
- E31: Vocabulary (school/family/animals)
- E32: Satzmuster (I like/have/can)
- E33: Questions
- E34: Mini-Reading
- E35: Mini-Writing

---

## Technische Details

- Reine HTML/CSS/JS (keine Frameworks)
- Offline-fahig nach erstem Laden
- Print-CSS fur sauberen A4-Export
- Keine externen Abhangigkeiten
- Keine Telemetrie, keine Analytics

---

## Lizenz

Frei zur Nutzung fur Bildungszwecke.
