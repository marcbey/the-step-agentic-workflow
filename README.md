# The Step

Vollständige Produkt- und Projektplanung für den Stuttgarter Skateboard e.V. / TheStep, Stand **22. Oktober 2026**.

**[GitHub-Projekt „The Step“ öffnen](https://github.com/users/marcbey/projects/4)**

Die Planung umfasst **13 Epics**, **91 ausgearbeitete Stories**, **547 konkrete Akzeptanzkriterien** und **5 Releases**. Alle fünf Anforderungsfotos, die bestehende Website und die verifizierten technischen Vorgaben aus „TheStep Verein“ sind berücksichtigt. Dies ist ein Planungsstand; die Anwendung wurde in diesem Repository noch nicht implementiert.

## Einstieg

1. [Produktkonzept, Zielgruppen und Abläufe](docs/planung/01-konzept.md)
2. [Quellen und vollständige Fotoabdeckung](docs/planung/02-quellen-und-abdeckung.md)
3. [Design und Inhaltsübernahme](docs/planung/03-design-und-inhalte.md)
4. [Architektur, Daten und Schnittstellen](docs/planung/04-architektur-und-daten.md)
5. [Roadmap, Prioritäten und Boardnutzung](docs/planung/05-roadmap-und-backlog.md)
6. [31 offene Fachentscheidungen und Risiken](docs/planung/06-entscheidungen-und-risiken.md)
7. [Qualität und Abnahme](docs/planung/07-qualitaet-und-abnahme.md)
8. [Alle Stories nach Epic](docs/planung/08-backlog-index.md)
9. [Umsetzungsübergabe nach Teilprojekten](docs/superpowers/plans/2026-10-22-the-step.md)
10. [Verifikation des GitHub-Planungsstands](docs/planung/09-verifikation.md)

## Lieferfolge

| Release | Schwerpunkt | Stories |
|---|---|---:|
| R0 | Fundament und verbindliche Entscheidungen | 6 |
| R1 | Website und Buchungsbetrieb | 45 |
| R2 | Verein und Team | 21 |
| R3 | Shop und Gutscheine | 9 |
| R4 | Optionale Erweiterungen | 10 |

Die Stories enthalten Nutzen, mindestens sechs prüfbare AKs, Abhängigkeiten, gezielte Prüfungen, technische Grenzen und Umsetzungsschritte. Punkte sind vorläufige relative Größen. Fachentscheidungen sind ausdrücklich offen; Termine und personelle Zusagen werden nicht erfunden. Alle Produktstories starten mit Todo.

## Referenz und Grenzen

Grunddesign und Informationsinhalte stammen aus der ausdrücklich genannten [TheStep-Website](https://thestep.schopp3r.de/). Ruby 4.0.6, Rails 8.1.3.1, SQLite, Hotwire und Kamal folgen dem fixierten Referenzstand des Projekts „TheStep Verein“. Neue Funktionen wie Mitgliedschaft, Shop und Rechnungen haben eigene Entscheidungen und Abnahmekriterien.

Die Planung enthält keine Zugangsdaten, Originalfotos, Produktivdaten oder ungeprüft übernommenen Medien. Ausgewählte Informationsseiten liegen als textliche Ausgangsstände unter `docs/planung/quellen/`; ihre Übernahme ist keine Freigabe für neue rechtliche oder steuerliche Prozesse.
