# 🦀 OpenClaw Dashboard v6

**Das interaktive Begleit-Dashboard zum Buch „Agentic Authorship: Mit n8n, Claude und OpenClaw zur automatisierten Buchfabrik"**

Das OpenClaw Dashboard führt dich Schritt für Schritt durch den Aufbau deiner eigenen KI-gestützten Buchproduktions-Pipeline – vom Server-Setup über Agent-Konfiguration bis zur Veröffentlichung auf Amazon KDP.

---

## 🚀 Live Demo

👉 **[tikitackr.github.io/OpenClaw-Dashboard](https://tikitackr.github.io/OpenClaw-Dashboard/)**

---

## ✨ Features

- **7 Module (Home + M1–M6)** – Strukturierter Weg vom leeren Server zum fertigen Buch
- **120 Tasks mit Fortschritts-Tracking** – Checkboxen, Fortschrittsbalken und Statistiken für jedes Modul
- **Personalisierte Code-Snippets** – Variablen-System ersetzt automatisch Server-IP, Domain, API-Keys etc. in allen Befehlen
- **Buch-Companion** – Alle 15 Kapitel mit Inline-Code-Snippets direkt im Dashboard
- **9 Sub-Agenten-Rollen** – Komplette MASTERPROMPT-Vorlagen (Content Architect, Technical Writer, Fact Checker u.v.m.)
- **X/Twitter Automation Pipeline** – Post-Workflow mit Telegram-Genehmigung, kein automatisches Posten
- **M6 „Dein Projekt"** – Agent-Team Generator und Dashboard-Konfigurator (in Entwicklung)
- **🐚 Cowan-Widget** – KI-Wissensassistentin als Floating-Chat direkt im Dashboard (BYOK mit Claude API)
- **Settings-Panel** – Eigene Daten einmal eingeben, überall in Code-Snippets verfügbar
- **localStorage-Persistenz** – Fortschritt und Einstellungen bleiben über Sessions erhalten
- **Responsive Design** – Optimiert für Desktop und Tablets (iPad 11" + Pro 14")

---

## 🛠 Technologie

- **React 18** – Komplett clientseitig, kein Backend nötig
- **Tailwind CSS** – Utility-first Styling via CDN
- **Lucide React** – 37 Icons, mit esbuild gebundelt
- **esbuild** – Build-Pipeline: JSX → Standalone HTML (189 KB)
- **GitHub Pages** – Kostenloses Hosting, Deploy aus `main` Branch
- **Claude API** – Für Cowan-Widget (Bring Your Own Key)

---

## 📖 Über das Buch

Das Dashboard ist der interaktive Begleiter zum Buch *„Agentic Authorship"* (EUR 39,95 auf Amazon KDP). Es bildet den gesamten Prozess ab, den das Buch beschreibt: Einen VPS einrichten, OpenClaw als Agent-Framework konfigurieren, Sub-Agenten für verschiedene Schreibaufgaben definieren, n8n-Workflows für Automatisierung nutzen und schließlich auf Amazon veröffentlichen.

---

## 📋 Die 7 Module

| Modul | Inhalt | Tasks |
|-------|--------|-------|
| **Home** | Projekt-Übersicht, Statistiken, Kapitel-Chart, Zeitplan | – |
| **M1 Server** | VPS-Setup, Docker, Tailscale, Domain | 18 |
| **M2 Agents** | Sub-Agenten-Rollen, SOUL.md, AGENTS.md | 10 |
| **M3 Automation** | n8n-Workflows, Trigger, X/Twitter-Pipeline | 10 |
| **M4 Publishing** | Amazon KDP, Cover, EPUB, Formatierung | 7 |
| **M5 Buch & Code** | 15 Kapitel mit Inline-Snippets + Settings | 75 |
| **M6 Dein Projekt** | Agent-Team Generator + Dashboard-Konfigurator | ★ |

---

## 🐚 Cowan – Die Buch-Instanz

Das Dashboard enthält **Cowan** als integriertes Floating-Widget – eine KI-Wissensassistentin, die Fragen zum Buch, zu OpenClaw, n8n und zur Claude API beantwortet. Cowan nutzt das BYOK-Prinzip (Bring Your Own Key): Du gibst deinen eigenen Claude API-Key ein und bezahlst nur deine eigenen API-Calls.

> 🔐 **Sicherheitshinweis:** Dein API-Key wird nur lokal in deinem Browser gespeichert und nie an Dritte übermittelt.

Cowan gibt es auch als **Standalone-App**: [tikitackr.github.io/Cowan](https://tikitackr.github.io/Cowan/)

---

## 🔧 Nutzung

1. Öffne das Dashboard: [tikitackr.github.io/OpenClaw-Dashboard](https://tikitackr.github.io/OpenClaw-Dashboard/)
2. Gehe zu **M5 → Meine Daten** und trage deine persönlichen Werte ein (Server-IP, Domain, API-Keys)
3. Arbeite die Module M1–M5 der Reihe nach durch – alle Code-Snippets sind automatisch personalisiert
4. Nutze den **🐚-Button** unten rechts, um Cowan bei Fragen zu öffnen (Claude API-Key nötig, ab $5 unter [console.anthropic.com](https://console.anthropic.com/settings/keys))

---

## 📁 Projektstruktur

```
dashboard/
├── index.html              # Fertige Standalone-Seite (189 KB) – deployed auf GitHub Pages
├── Dashboard_v6.jsx        # React-Quellcode (107 KB, 2047 Zeilen)
├── cowan-widget.jsx         # Cowan Chat-Widget (1064 Zeilen)
├── build-dashboard.js       # esbuild Build-Script
├── package.json             # Dependencies (React, esbuild, lucide-react)
├── README.md                # Diese Datei
├── _archive/                # Ältere Dashboard-Versionen (v1–v5)
└── node_modules/            # Dependencies
```

---

## 🗺 Roadmap

- ☐ M6 Agent-Team Generator aktivieren (API-Anbindung)
- ☐ M6 Dashboard-Konfigurator (Prompt-Generator)
- ☐ Echte Buchinhalte in Cowan-Wissensbasis einfügen
- ☐ Konfetti-Animation bei 100% Fortschritt
- ☐ Print-Ansicht für Offline-Nutzung

---

## Lizenz

MIT

Erstellt mit [Claude](https://claude.ai) von [Anthropic](https://anthropic.com)
