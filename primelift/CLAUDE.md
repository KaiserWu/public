# PRimeLift – Rechtliche Dokumente & Landing-Page

## App-Beschreibung

**PRimeLift** (Repo: `Exercises-Tracker`, Bundle-ID `de.LP.wus.Exercises-Tracker`) ist eine
native App für Krafttraining, iOS 26.5 + watchOS 26.5.

**Kernfunktionen:**
- Trainingspläne aus einem Übungskatalog (127 Kernübungen, 1.324 gesamt) plus eigene Übungen
- Training protokollieren: Sätze, Pausen-Timer, PR-Erkennung
- Statistik: geschätztes 1RM, Wochenvolumen, harte Sätze je Muskelgruppe
- Apple-Watch-App mit Digital Crown, Pausen-Ring und HealthKit-Workout
- Optionaler KI-Coach (Anthropic, OpenAI, Gemini, MiniMax, eigener Endpunkt, Apple Intelligence)
- Deutsch und Englisch

**Entwickler:** Sen Wu / ThinkWu
**Plattform:** iOS + watchOS (SwiftUI + SwiftData + CloudKit)

## Inhalt dieses Ordners

| Datei | Inhalt |
|-------|--------|
| `index.html` | Landing-Page (Deutsch, mit englischer Kurzfassung) |
| `datenschutz-de.html` / `-en.html` | Datenschutzerklärung |
| `nutzungsbedingungen-de.html` / `-en.html` | Nutzungsbedingungen |
| `support-de.html` / `-en.html` | Support-Seite mit FAQ |

Dateinamen folgen dem Muster von `quick-food-tracker/` (deutsche Namen mit
Sprach-Suffix), nicht dem „Dateinamen auf Englisch" aus der Root-`CLAUDE.md` — im
Zweifel zählt die Konsistenz mit der Schwester-App.

## Für die App-Store-Einreichung

| Feld | URL |
|---|---|
| Privacy Policy URL (Pflicht) | `.../primelift/datenschutz-en.html` |
| Support URL (Pflicht) | `.../primelift/support-en.html` |
| Marketing URL (optional) | `.../primelift/index.html` |
| EULA (optional) | `.../primelift/nutzungsbedingungen-en.html` |

Basis: `https://kaiserwu.github.io/public/`

## Hinweise zur Pflege

**Die Datenschutzerklärung gibt es zweimal** — hier als HTML und in der App unter
Einstellungen → Datenschutz (`LegalDocumentView`, Inhalt in
`Views/Settings/LegalDocumentView.swift`). Das ist bewusst so: Wer im Studio wissen
will, was mit seinen Daten passiert, hat dort oft kein Netz. Der Preis ist, dass
**beide Fassungen gemeinsam geändert werden müssen** — dasselbe gilt für die
Nutzungsbedingungen.

Was eine Aktualisierung erzwingt:

- neue Datenerhebung oder neue Berechtigung (z. B. Standort, Mikrofon)
- ein neuer KI-Anbieter oder eine geänderte Übertragung an bestehende
- Änderungen daran, was über iCloud synchronisiert wird
- neue Fremdbibliotheken — die App hat derzeit **keine**, und genau das steht so in
  der Erklärung; sobald sich das ändert, wird die Aussage falsch

Beide Sprachfassungen inhaltlich gleich halten und den Stand mitziehen.
