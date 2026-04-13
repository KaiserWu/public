# CLAUDE.md

## Zweck

Dieses Repo hostet statische HTML-Seiten für private Apps via GitHub Pages.

## Struktur

```
/
├── impressum-de.html       # Impressum (bleibt in root)
├── impressum-en.html
├── <app-name>/             # Jede App bekommt einen eigenen Ordner
│   ├── datenschutz-de.html
│   ├── datenschutz-en.html
│   └── ...
└── README.md
```

- **Impressum** bleibt in root
- **Jede App** bekommt einen eigenen Unterordner (z.B. `quick-food-tracker/`)
- Dateinamen auf Englisch, Inhalt je nach Sprache
- Kein Build-Prozess, kein Framework – nur statisches HTML

## Bestehende Apps

- `quick-food-tracker/` – Datenschutzerklärungen für QuickFoodTracker
