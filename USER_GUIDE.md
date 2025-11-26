# 📖 Benutzerhandbuch - Call of Duty Spieler-Treffpunkt

Willkommen zum vollständigen Benutzerhandbuch für die Gaming-Plattform!

## 🚀 Schnellstart

1. **Server starten:**
   ```bash
   yarn start
   ```

2. **Browser öffnen:**
   - Öffne `http://localhost:XXXX` (Port wird im Terminal angezeigt)

3. **Loslegen:**
   - Erkunde bestehende Sessions
   - Erstelle deine erste Session
   - Trete einer Session bei

---

## 📝 Inhaltsverzeichnis

1. [Sessions verwalten](#sessions-verwalten)
2. [Suchen & Filtern](#suchen--filtern)
3. [Theme wechseln](#theme-wechseln)
4. [Statistiken ansehen](#statistiken-ansehen)
5. [Daten exportieren/importieren](#daten-exportierenimportieren)
6. [Keyboard-Shortcuts](#keyboard-shortcuts)
7. [Tipps & Tricks](#tipps--tricks)
8. [Häufige Fragen (FAQ)](#häufige-fragen-faq)
9. [Fehlerbehebung](#fehlerbehebung)

---

## 📋 Sessions verwalten

### ➕ Session erstellen

1. **Formular öffnen:**
   - Klicke auf den Button "➕ Neue Session" in der Controls-Bar
   - ODER drücke `Ctrl/Cmd + N`

2. **Felder ausfüllen:**
   
   **Pflichtfelder (*):**
   - **Session-Name**: Gib deiner Session einen aussagekräftigen Namen
     - Beispiel: "Warzone Abend-Session", "Ranked Grinding"
   
   - **Spielmodus**: Wähle einen Modus aus
     - Warzone
     - Multiplayer
     - Zombies
     - Ranked
     - Custom Match
   
   - **Dein Name**: Wie willst du genannt werden?
     - Beispiel: "GamerPro42", "CoD_Legend"
   
   - **Max. Spieler**: Wie viele Spieler können mitmachen?
     - Min: 2, Max: 150
     - Standard: 4
   
   - **Skill-Level**: Welches Niveau erwartest du?
     - Anfänger
     - Casual
     - Fortgeschritten
     - Profi
     - Alle Level
   
   - **Plattform**: Auf welcher Plattform spielst du?
     - PC
     - PlayStation
     - Xbox
     - Cross-Platform
   
   - **Startzeit**: Wann beginnt die Session?
     - Wähle Datum und Uhrzeit
   
   **Optional:**
   - **Beschreibung**: Zusätzliche Infos
     - Discord-Link
     - Besondere Anforderungen
     - Was du von Mitspielern erwartest

3. **Session erstellen:**
   - Klicke auf "Session erstellen"
   - ✅ Toast-Benachrichtigung erscheint
   - Session wird sofort in der Liste angezeigt

4. **Abbrechen:**
   - Klicke auf "Abbrechen" um das Formular zu schließen
   - ODER drücke das "X" oder klicke außerhalb

---

### 🔍 Session ansehen

**Session-Card aufgebaut:**

```
┌─────────────────────────────────────┐
│ 🗑️ Löschen (on hover)              │
│                                     │
│ [Session-Name]         [Modus-Tag] │
│                                     │
│ Host: GamerName    Startzeit: 20:00│
│ Skill: Casual      Plattform: PC   │
│                                     │
│ Beschreibung...                     │
│                                     │
├─────────────────────────────────────┤
│ 👥 2/4 Spieler        [Beitreten]  │
└─────────────────────────────────────┘
```

**Details ansehen:**
- Klicke irgendwo auf die Card (außer Buttons)
- Modal öffnet sich mit vollständigen Details
- Schließen: Klicke X, drücke ESC, oder klicke außerhalb

---

### ✅ Session beitreten

**Methode 1 - Von der Card:**
1. Finde eine passende Session
2. Klicke auf "Beitreten"-Button
3. ✅ Toast-Benachrichtigung erscheint
4. Spieleranzahl aktualisiert sich automatisch

**Methode 2 - Aus dem Modal:**
1. Klicke auf eine Session-Card
2. Prüfe die Details
3. Klicke auf "Jetzt beitreten"

**Status-Anzeige:**
- 🟢 **Verfügbar**: "Beitreten"-Button ist grün/türkis
- 🔴 **Voll**: Button ist grau und disabled

---

### 🗑️ Session löschen

1. **Delete-Button anzeigen:**
   - Fahre mit der Maus über eine Session-Card
   - 🗑️-Button erscheint oben rechts

2. **Löschen:**
   - Klicke auf den 🗑️-Button
   - Confirmation-Dialog erscheint
   - Bestätige oder breche ab

3. **Gelöscht:**
   - ✅ Toast-Benachrichtigung erscheint
   - Session verschwindet aus der Liste
   - Wird auch aus LocalStorage entfernt

**Hinweis:** Gelöschte Sessions können nicht wiederhergestellt werden (außer via Import).

---

## 🔍 Suchen & Filtern

### Echtzeit-Suche

1. **Suche aktivieren:**
   - Klicke in das Suchfeld
   - ODER drücke `Ctrl/Cmd + K`

2. **Suchbegriff eingeben:**
   - Sessions werden live gefiltert
   - Sucht in: Name, Host, Beschreibung
   - Case-insensitive

3. **Suche löschen:**
   - Lösche den Text im Suchfeld
   - Alle Sessions werden wieder angezeigt

**Beispiele:**
- "warzone" → Findet alle Warzone-Sessions
- "pro" → Findet "GamerPro42", "Profi", etc.
- "discord" → Findet Sessions mit Discord in Beschreibung

---

### Filter nach Modus

**Filter-Buttons in der Controls-Bar:**

```
[Alle] [Warzone] [Multiplayer] [Zombies] [Ranked]
```

1. **Filter auswählen:**
   - Klicke auf einen Filter-Button
   - Button wird hervorgehoben (Active-State)

2. **Filter zurücksetzen:**
   - Klicke auf "Alle"

**Kombination mit Suche:**
- Filter + Suche = UND-Verknüpfung
- Beispiel: Filter "Warzone" + Suche "casual"
  → Zeigt nur casual Warzone-Sessions

---

### Sortierung

**Sortier-Dropdown:**

```
[Neueste zuerst ▼]
```

**4 Optionen:**

1. **Neueste zuerst** (Standard)
   - Zuletzt erstellte Sessions zuerst
   - Gut für aktuelle Sessions

2. **Älteste zuerst**
   - Älteste Sessions zuerst
   - Nützlich für historische Ansicht

3. **Wenigste Spieler**
   - Sessions mit wenigen Teilnehmern zuerst
   - Gut für schnellen Beitritt

4. **Meiste Spieler**
   - Beliebte Sessions zuerst
   - Zeigt, wo Action ist

**Wählen:**
- Klicke auf das Dropdown
- Wähle eine Option
- Liste aktualisiert sich sofort

---

## 🌓 Theme wechseln

### Dark Mode ↔️ Light Mode

**Button im Header:**

```
[🌙] oder [☀️]
```

1. **Theme wechseln:**
   - Klicke auf den Theme-Toggle-Button
   - Icon wechselt zwischen 🌙 und ☀️

2. **Automatisch gespeichert:**
   - Deine Präferenz wird gespeichert
   - Beim nächsten Besuch wird sie geladen

**Eigenschaften:**

**Dark Mode (Standard):**
- Dunkle Hintergründe
- Hoher Kontrast
- Gaming-optimiert
- Augenfreundlich bei Nacht

**Light Mode:**
- Helle Oberfläche
- Weiche Farben
- Gut bei Tageslicht
- Modern & clean

---

## 📊 Statistiken ansehen

### Statistik-Dashboard öffnen

**3 Wege:**
1. Klicke auf "📊 Stats"-Button
2. Drücke `Ctrl/Cmd + S`
3. Klicke Footer-Link (wenn implementiert)

### Dashboard-Übersicht

**4 Metriken-Karten:**

```
┌─────────────┐ ┌─────────────┐
│      X      │ │      Y      │
│ Gesamt      │ │ Gesamt      │
│ Sessions    │ │ Spieler     │
└─────────────┘ └─────────────┘

┌─────────────┐ ┌─────────────┐
│     X.X     │ │      Z      │
│ Ø Spieler/  │ │ Volle       │
│ Session     │ │ Sessions    │
└─────────────┘ └─────────────┘
```

**Modus-Statistik:**
- Liste mit Count pro Spielmodus
- Zeigt beliebteste Modi

**Modal schließen:**
- Klicke X, ESC, oder außerhalb

---

## 💾 Daten exportieren/importieren

### 📤 Export

**Sessions exportieren:**

1. **Export starten:**
   - Klicke auf "💾 Export"-Button
   - Oder benutze Menü

2. **Datei speichern:**
   - Browser-Download-Dialog öffnet sich
   - Dateiname: `cod-sessions-YYYY-MM-DD.json`
   - Speichere die Datei

3. **Bestätigung:**
   - ✅ Toast-Benachrichtigung erscheint

**Use-Cases:**
- Backup erstellen
- Sessions mit Freunden teilen
- Zwischen Browsern migrieren

---

### 📥 Import

**Sessions importieren:**

1. **Import starten:**
   - Klicke auf "📥 Import"-Button
   - File-Picker öffnet sich

2. **Datei auswählen:**
   - Wähle eine `.json`-Datei
   - Nur gültige Session-Dateien werden akzeptiert

3. **Import-Modus wählen:**
   - **Dialog erscheint:**
     - "OK" = Zusammenführen mit bestehenden
     - "Abbrechen" = Alle Sessions ersetzen

4. **Import abgeschlossen:**
   - ✅ Toast zeigt Anzahl importierter Sessions
   - Sessions erscheinen in der Liste

**Fehlerbehandlung:**
- Bei ungültigen Dateien: ❌ Error-Toast
- Format muss JSON-Array sein

---

## ⌨️ Keyboard-Shortcuts

### Übersicht

| Shortcut | Aktion | Beschreibung |
|----------|--------|--------------|
| `Ctrl + K` (Mac: `Cmd + K`) | 🔍 Suche fokussieren | Cursor springt ins Suchfeld |
| `Ctrl + N` (Mac: `Cmd + N`) | ➕ Neue Session | Öffnet Erstellungs-Formular |
| `Ctrl + S` (Mac: `Cmd + S`) | 📊 Statistiken | Öffnet Stats-Dashboard |
| `ESC` | ❌ Modal schließen | Schließt offenes Modal/Dialog |

### Verwendung

**Workflow-Beispiel:**

1. `Ctrl + K` → Suche nach "warzone"
2. Finde passende Session
3. Klicke zum Beitreten
4. `Ctrl + S` → Prüfe Statistiken
5. `ESC` → Schließe Stats

**Vorteile:**
- ⚡ Schnellere Navigation
- 🖱️ Maus nicht immer nötig
- 💪 Power-User-freundlich

---

## 💡 Tipps & Tricks

### Effizienz-Tipps

1. **Keyboard-Shortcuts nutzen:**
   - Lerne die Shortcuts auswendig
   - Spare Zeit bei häufigen Aktionen

2. **Filter clever kombinieren:**
   - Modus-Filter + Suche + Sortierung
   - Finde genau was du suchst

3. **Beschreibung nutzen:**
   - Füge Discord-Link hinzu
   - Erwähne besondere Anforderungen
   - Beschreibe deinen Spielstil

4. **Theme anpassen:**
   - Wechsle je nach Tageszeit
   - Dark Mode abends
   - Light Mode tagsüber

### Beste Praktiken

**Session-Namen:**
✅ **Gut:**
- "Warzone Trios - Entspannt 🎮"
- "Ranked Push - Diamond+ 💎"
- "Zombies Marathon EE 🧟"

❌ **Schlecht:**
- "Spiel"
- "123"
- "asdfgh"

**Beschreibungen:**
✅ **Gut:**
- "Suche 2 Spieler für entspannte Trios. Discord vorhanden. Kein Rage, nur Fun!"
- "Ranked Push zum Master. Min. Diamond-Rang. Gute Kommunikation Pflicht."

❌ **Schlecht:**
- "..."
- "Spiel"
- Leer lassen

**Startzeiten:**
✅ **Gut:**
- Realistische Zeiten wählen
- Puffer einplanen

❌ **Schlecht:**
- Zeit in der Vergangenheit
- Zu weit in der Zukunft

### Organisation

1. **Regelmäßig aufräumen:**
   - Alte Sessions löschen
   - Auto-Cleanup nutzen (läuft automatisch)

2. **Backup erstellen:**
   - Exportiere Sessions regelmäßig
   - Speichere Backup-Dateien sicher

3. **Sessions kategorisieren:**
   - Nutze konsistente Namenskonventionen
   - Verwende Emojis für schnelle Erkennung

---

## ❓ Häufige Fragen (FAQ)

### Allgemein

**Q: Werden meine Daten gespeichert?**
- A: Ja, lokal im Browser (LocalStorage). Keine Server-Kommunikation.

**Q: Kann ich Sessions mit anderen teilen?**
- A: Ja, über Export/Import-Funktion als JSON-Datei.

**Q: Funktioniert die App offline?**
- A: Ja, nach dem ersten Laden. Keine Internet-Verbindung nötig.

**Q: Sind Sessions zwischen Browsern synchronisiert?**
- A: Nein, nur lokal pro Browser. Nutze Export/Import für Sync.

### Sessions

**Q: Was passiert mit vollen Sessions?**
- A: Beitreten-Button wird disabled. Kann nicht mehr beitreten.

**Q: Kann ich eine Session bearbeiten?**
- A: Aktuell nicht. Lösche und erstelle neu.

**Q: Wo ist meine Session hin?**
- A: Auto-Cleanup entfernt Sessions älter als 24h. Nutze Export für Backup.

**Q: Wie viele Sessions kann ich erstellen?**
- A: Unbegrenzt (technisch durch LocalStorage limitiert: ~5-10MB).

### Suche & Filter

**Q: Warum finde ich keine Sessions?**
- A: Prüfe Filter-Einstellungen und Suchbegriff. Klicke "Alle" für Reset.

**Q: Case-sensitive Suche?**
- A: Nein, Groß-/Kleinschreibung wird ignoriert.

**Q: Mehrere Filter gleichzeitig?**
- A: Ein Modus-Filter + Suche + Sortierung ist möglich.

### Import/Export

**Q: Welches Format für Import?**
- A: JSON-Array mit Session-Objekten. Siehe exportierte Datei als Beispiel.

**Q: Import überschreibt Sessions?**
- A: Du wirst gefragt: Zusammenführen oder Ersetzen.

**Q: Kann ich Sessions manuell bearbeiten?**
- A: Ja, bearbeite die JSON-Datei und importiere neu.

---

## 🔧 Fehlerbehebung

### Probleme & Lösungen

#### Problem: Sessions werden nicht gespeichert

**Mögliche Ursachen:**
- LocalStorage deaktiviert
- Private/Incognito-Modus
- Browser-Limit erreicht

**Lösungen:**
1. Prüfe Browser-Einstellungen
2. Verlasse Private-Modus
3. Lösche alte Sessions
4. Exportiere Sessions regelmäßig

---

#### Problem: Suche findet nichts

**Lösungen:**
1. Prüfe Suchbegriff auf Tippfehler
2. Klicke "Alle"-Filter
3. Leere Suchfeld
4. Lade Seite neu (F5)

---

#### Problem: Theme wechselt nicht

**Lösungen:**
1. Lade Seite neu
2. Prüfe Browser-Konsole auf Fehler
3. Lösche LocalStorage:
   ```javascript
   // In Browser-Konsole:
   localStorage.removeItem('theme');
   location.reload();
   ```

---

#### Problem: Import funktioniert nicht

**Lösungen:**
1. Prüfe Dateiformat (muss JSON sein)
2. Validiere JSON-Struktur
3. Nutze exportierte Datei als Vorlage
4. Prüfe Browser-Konsole auf Fehler

---

#### Problem: App lädt nicht

**Lösungen:**
1. Prüfe Server-Status (Terminal)
2. Starte Server neu:
   ```bash
   # Terminal: Ctrl+C zum Stoppen
   yarn start  # Neu starten
   ```
3. Prüfe Port (eventuell belegt)
4. Lösche Browser-Cache

---

### Browser-Konsole öffnen

**Chrome/Edge/Firefox:**
- Windows/Linux: `F12` oder `Ctrl + Shift + I`
- Mac: `Cmd + Option + I`

**Safari:**
1. Aktiviere Entwickler-Menü in Einstellungen
2. `Cmd + Option + I`

---

### LocalStorage löschen

**Alle Daten zurücksetzen:**

```javascript
// Browser-Konsole (F12):
localStorage.clear();
location.reload();
```

**Nur Sessions löschen:**

```javascript
localStorage.removeItem('codSessions');
location.reload();
```

⚠️ **Warnung:** Erstelle vorher ein Export-Backup!

---

## 📞 Support

### Selbsthilfe

1. ✅ Lies diese Anleitung
2. ✅ Prüfe [FAQ](#häufige-fragen-faq)
3. ✅ Siehe [Fehlerbehebung](#fehlerbehebung)

### Community

- Discord: CoD-Treffpunkt#1234
- E-Mail: info@cod-treffpunkt.de
- GitHub: [Repository-Link]

### Feedback

Wir freuen uns über:
- Bug-Reports
- Feature-Requests
- Verbesserungsvorschläge
- Allgemeines Feedback

---

## 📚 Weitere Ressourcen

- [README.md](README.md) - Projekt-Übersicht
- [FEATURES.md](FEATURES.md) - Detaillierte Feature-Liste
- [CHANGELOG.md](CHANGELOG.md) - Versions-Historie

---

**Viel Erfolg beim Finden deiner Gaming-Buddies! 🎮🔥**

**Letzte Aktualisierung:** November 2025
