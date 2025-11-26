# Call of Duty - Spieler-Treffpunkt

Eine minimalistische Gaming-Plattform für Call of Duty Spieler, um gemeinsame Gaming-Sessions zu finden und zu organisieren.

## 🎮 Features

- **Moderne UI**: Minimalistisches, dunkles Design mit Gaming-Ästhetik
- **Responsive Design**: Funktioniert auf Desktop, Tablet und Mobile
- **Session-Übersicht**: Zeigt offene Gaming-Sessions mit Details
- **Session-Erstellung**: Formular zum Erstellen neuer Sessions (UI-Platzhalter)
- **Semantisches HTML5**: Verwendet moderne HTML5-Elemente
- **Reines HTML/CSS**: Keine JavaScript-Abhängigkeiten

## 🚀 Installation & Start

### Voraussetzungen

- Node.js und Yarn installiert

### Mit Yarn starten

```bash
# Dependencies installieren (optional, da wir npx verwenden)
yarn install

# Entwicklungsserver starten
yarn start
```

Der Server startet standardmäßig auf `http://localhost:3000`

### Alternative Start-Befehle

```bash
# Mit yarn dev
yarn dev

# Mit yarn serve
yarn serve
```

## 📁 Projekt-Struktur

```
/workspace/
├── index.html      # Hauptdatei mit HTML & CSS
├── package.json    # Yarn-Konfiguration
└── README.md       # Diese Datei
```

## 🎨 Design-Features

- **Dark Theme**: Gaming-optimierte Farbpalette
- **Gradient-Backgrounds**: Moderne visuelle Effekte
- **Hover-Effekte**: Interaktive UI-Elemente
- **Card-Layout**: Übersichtliche Session-Darstellung
- **Responsive Grid**: Passt sich an verschiedene Bildschirmgrößen an

## 📱 Responsive Breakpoints

- **Desktop**: > 768px
- **Tablet**: 481px - 768px
- **Mobile**: < 480px

## 🛠️ Technologie-Stack

- **HTML5**: Semantische Markup-Struktur
- **CSS3**: Modernes Styling mit Flexbox & Grid
- **Serve**: Einfacher HTTP-Server für lokale Entwicklung

## 💡 UI-Komponenten

### Header
- Plattform-Titel
- Untertitel/Beschreibung

### Main Section
- **Session-Erstellung**: Formular mit Feldern für:
  - Session-Name
  - Spielmodus
  - Maximale Spieleranzahl
  - Startzeit
  - Beschreibung
  
- **Session-Liste**: Karten mit:
  - Session-Titel & Modus
  - Host-Information
  - Startzeit
  - Skill-Level
  - Plattform
  - Spieleranzahl
  - Beitreten-Button

### Footer
- Copyright-Information
- Navigations-Links

## 🎯 Verwendungszweck

Diese Anwendung ist ein reiner Frontend-Prototyp ohne Backend-Funktionalität. 
Alle Formulare und Buttons sind UI-Platzhalter ohne tatsächliche Funktionalität.

## 📝 Hinweise

- Die Anwendung ist für lokale Entwicklung optimiert
- Keine Datenbank oder Backend erforderlich
- Keine JavaScript-Funktionalität implementiert
- Ideal für Design-Prototyping und Konzeptdarstellung

## 🌐 Browser-Kompatibilität

- Chrome/Edge (neueste Versionen)
- Firefox (neueste Versionen)
- Safari (neueste Versionen)

---

**Hinweis**: Dies ist eine reine Frontend-Demo ohne Backend-Funktionalität.
