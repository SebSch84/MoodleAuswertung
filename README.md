# Klassenarbeit Auswertung Tool

Ein lokales Browser-Tool zur Auswertung von Klassenarbeiten aus Moodle-/ODS-Exporten. Entwickelt für das BBZ am Nord-Ostsee-Kanal.
*Vibe coded*

## Features

- 📂 **ODS / XLSX Upload** per Drag & Drop
- 📐 **Drei Notenspiegel** wählbar: Linear (Schule), IHK, Individuell
- 🎯 **Tendenz-Noten** (z. B. 2+, 3−) und Dezimalnoten zur Kontrolle
- 🖨 **Einzelausdrucke** pro Schüler mit Schullogo und Unterschriftsfeldern
- 📋 **Notenübersicht** mit Klassenstatistik, Notenverteilung und Tabelle
- 🔒 **100 % lokal** – keine Daten verlassen den Browser, kein Server nötig

## Voraussetzungen

- Keine Installation nötig
- Funktioniert in jedem modernen Browser (Chrome, Firefox, Edge, Safari)
- Beim ersten Öffnen wird eine Schriftart von Google Fonts geladen (optional, funktioniert auch offline mit Fallback-Schrift)

## Dateiformat

Die ODS-Datei muss folgende Spalten enthalten:

| Spalte | Beispiel |
|--------|---------|
| Nachname | Mustermann |
| Vorname | Max |
| Bewertung/39,00 | 28,50 |
| F 1 /1,00 | 1 |
| F 2 /3,00 | 2,50 |
| … | … |

Zusätzliche Spalten (E-Mail, Begonnen, Beendet, Verbrauchte Zeit) werden automatisch erkannt und auf dem Ausdruck angezeigt.

## Benutzung

1. `Klassenarbeit_Tool.html` herunterladen
2. Datei im Browser öffnen (Doppelklick)
3. Titel der Klassenarbeit eingeben
4. Notenspiegel wählen (Linear / IHK / Individuell)
5. ODS-Datei per Drag & Drop hochladen
6. **🖨 Einzelausdrucke** → druckt ein Blatt pro Schüler
7. **📋 Notenübersicht drucken** → druckt die Klassenübersicht

## Datenschutz

- Alle Daten werden ausschließlich lokal im Browser verarbeitet
- Es werden keine Schülerdaten an Server übertragen oder gespeichert
- Das Tool ist geeignet für den schulischen Einsatz gemäß DSGVO

---

## Repository einrichten (Schritt-für-Schritt)

### 1. GitHub-Account

Falls noch nicht vorhanden: [github.com](https://github.com) → „Sign up"

### 2. Neues Repository anlegen

1. Auf GitHub einloggen
2. Oben rechts auf **„+"** → **„New repository"**
3. Name eingeben, z. B. `klassenarbeit-tool`
4. **Private** wählen (empfohlen) oder Public
5. „Create repository" klicken

### 3. Dateien hochladen

**Option A – direkt im Browser (einfacher):**
1. Im neuen Repository auf **„uploading an existing file"** klicken
2. `Klassenarbeit_Tool.html` und `README.md` hineinziehen
3. Unten auf **„Commit changes"** klicken

**Option B – per Git (für Fortgeschrittene):**
```bash
git clone https://github.com/DEINNAME/klassenarbeit-tool.git
# Dateien in den Ordner kopieren
git add .
git commit -m "Klassenarbeit Tool hinzugefügt"
git push
```

### 4. Mit Kollegen teilen

**Privates Repository:**
1. Repository → **Settings** → **Collaborators**
2. **„Add people"** → E-Mail oder GitHub-Nutzername eingeben
3. Kollege erhält eine Einladung per E-Mail

**Öffentliches Repository (alternativ):**
- Einfach den Link zum Repository teilen, z. B.:  
  `https://github.com/DEINNAME/klassenarbeit-tool`
- Jeder kann die Datei dann herunterladen

### 5. GitHub Pages (optional – Tool direkt im Browser nutzbar)

Wenn das Repository **öffentlich** ist:
1. Repository → **Settings** → **Pages**
2. Source: **„Deploy from a branch"**
3. Branch: **main** → Ordner: **/ (root)**
4. **Save** klicken
5. Nach 1–2 Minuten ist das Tool erreichbar unter:  
   `https://DEINNAME.github.io/klassenarbeit-tool/Klassenarbeit_Tool.html`

Diesen Link kannst du dann direkt an Kollegen schicken – kein Download nötig.
