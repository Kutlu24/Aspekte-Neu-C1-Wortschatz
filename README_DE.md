# 🇩🇪 Deutsch Vokabeltrainer - Web-Anwendung

Eine moderne, responsive und benutzerfreundliche Plattform zum Deutschlernen.

## ✨ Funktionen

### 📇 Lernkarten-Modus
- Wörter als Vorder-/Rückseite-Karten anzeigen
- Karte umdrehen, um Grammatikregeln und Beispielsätze zu sehen
- Gelernte Wörter markieren und Fortschritt verfolgen

### 🎯 Quiz-Modus
- Beispielsatz-Zuordnungs-Quiz
- Automatische Punkteberechnung
- Sofortiges Feedback (richtig/falsch)

### 🔊 Audio-Funktionen
- Aussprache für jedes Wort
- Hochwertige Audiodateien im Opus-Format
- Audio mit einem Klick abspielen

### 🎨 Filtern und Suchen
- Nach Lektion filtern (1-10)
- Nach Teil filtern (1-8)
- Suche in Wörtern, Grammatik oder Beispielsätzen
- Zufällige Sortierung

### 💾 Fortschrittsverfolgung
- Gelernte Wörter werden im Browser gespeichert
- Statistiken: Gesamt/Gelernt/Übrig Wortanzahl
- Funktion zum Zurücksetzen des Fortschritts

### ⌨️ Tastaturkürzel
- `←` / `→` : Vorheriges/Nächstes Wort
- `Leertaste` : Karte umdrehen
- `Enter` : Audio abspielen

## 📊 Statistiken

- **Wörter gesamt**: 626
- **Anzahl Lektionen**: 10
- **Anzahl Teile**: 8
- **Audiodateien**: 327

## 🚀 Verwendung

### Lokale Nutzung

1. Laden Sie die Dateien in diesem Ordner herunter
2. Öffnen Sie die Datei `index.html` in einem Webbrowser
3. Beginnen Sie mit dem Lernen!

**Hinweis**: Damit die Audiodateien funktionieren, müssen Sie die Dateien möglicherweise auf einem Webserver ausführen.

### Mit Webserver (Empfohlen)

Einfacher Webserver mit Python 3:
```bash
python -m http.server 8000
```

Dann in Ihrem Browser: `http://localhost:8000`

### Mit GitHub Pages (Beste Lösung)

Kostenlos und einfach! Detaillierte Anweisungen finden Sie in der Datei `DEPLOYMENT.md`.

## 🗄️ Archiv

Dieses Repository ist die aktuelle, gepflegte Version. Eine frühere, kleinere Version mit ähnlichem Thema (`HEY-Bist-Du-Bereit---C1`) ist zur Referenz unter [`archive/v1-hey-bist-du-bereit-c1/`](archive/v1-hey-bist-du-bereit-c1/) abgelegt und wird nicht mehr separat gepflegt.

## 📁 Dateistruktur

```
.
├── index.html              # Haupt-Webanwendung (einzelne Datei)
├── kelimeler_web.json      # Wortdatenbank (626 Wörter)
├── sesler/                 # Audio-Dateien Ordner
│   ├── 1.opus
│   ├── 2.opus
│   └── ... (327 Dateien)
├── vokabelliste-web-14.2.2026.xlsx  # Quell-Excel-Datei
├── README.md               # Diese Datei (Türkisch)
├── README_DE.md            # Diese Datei (Deutsch)
└── DEPLOYMENT.md           # GitHub Pages Installationsanleitung
```

## 🛠️ Technische Details

### Technologien
- **Frontend**: Pure HTML5, CSS3, JavaScript (ES6+)
- **Design**: Modernes Gradient-Design, responsive Layout
- **Daten**: JSON-Format Wortdatenbank
- **Audio**: Opus-Format (unterstützt von Chrome, Firefox, Edge)

### Browser-Kompatibilität
- ✅ Chrome/Edge (empfohlen)
- ✅ Firefox
- ✅ Safari
- ✅ Mobile Browser (iOS Safari, Chrome Mobile)

### Responsive Design
- 📱 Mobiltelefone
- 📱 Tablets
- 💻 Desktop-Computer

## 🎓 Wortdatenbank

Wörter werden aus der Excel-Datei (`vokabelliste-web-14.2.2026.xlsx`) in das JSON-Format konvertiert.

### Datenstruktur
```json
{
  "id": 1,
  "wort": "schiefgehen",
  "grammatik": "geht schief, ging schief, ist schiefgegangen",
  "beispiel": "Gestern ging wirklich alles schief – was für ein Tag!",
  "lektion": 1,
  "audio": "1.opus",
  "teil": 1
}
```

### Neue Wörter hinzufügen

1. Bearbeiten Sie die Excel-Datei
2. Konvertieren Sie sie mit dem Python-Skript in JSON:

```python
import pandas as pd
import json

df = pd.read_excel('vokabelliste-web-14.2.2026.xlsx')
# ... (Code in DEPLOYMENT.md)
```

## 🎨 Anpassung

### Farben ändern
Im CSS-Abschnitt in `index.html`:
```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

### Neue Funktionen hinzufügen
Durch Bearbeiten des JavaScript-Abschnitts:
- Verschiedene Quiz-Typen
- Spaced Repetition Algorithmus
- Mehrsprachige Unterstützung
- usw.

## 📝 Lizenz

Dieses Projekt wurde für den persönlichen Gebrauch entwickelt.

## 🤝 Mitwirken

1. Fork erstellen
2. Feature-Branch erstellen (`git checkout -b feature/neueFunktion`)
3. Commit erstellen (`git commit -m 'Neue Funktion hinzugefügt'`)
4. Push durchführen (`git push origin feature/neueFunktion`)
5. Pull Request öffnen

## 📧 Kontakt

Für Fragen können Sie GitHub Issues verwenden.

---

**Made with ❤️ for German language learners**

🇩🇪 Viel Erfolg beim Deutschlernen! 🎓
