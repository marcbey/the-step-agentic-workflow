# Prüfung des veröffentlichten Planungsstands

Stand: 22. Oktober 2026. Gegenstand ist die vollständige Planung, nicht die Produktimplementierung.

| Prüfung | Nachgewiesenes Ergebnis |
|---|---|
| Repository-Issues | 104 offene Issues: 13 Epics und 91 Stories |
| Akzeptanzkriterien | 547 nummerierte AKs in den Story-Issues und lokalen Storydateien |
| Native Unteraufgaben | Alle 91 Stories gehören zum vorgesehenen Epic; die Mengen wurden für jedes der 13 Epics über die GitHub-API verglichen |
| Meilensteine | R0: 6, R1: 45, R2: 21, R3: 9, R4: 10 Stories; keine bereits geschlossene Produktstory |
| Prioritäten und Bereiche | Alle Stories haben passende Labels; offene Fachentscheidungen sind gekennzeichnet |
| Abhängigkeiten | Alle referenzierten Story-IDs existieren; keine Zyklen und keine fachliche Abhängigkeit auf ein späteres Release |
| Quellenabdeckung | Alle lesbaren Themen der fünf Fotos sind im Quellenregister einer oder mehreren Stories zugeordnet |
| Inhalt und Design | Fünf angeforderte Informationsseiten als Text-Ausgangsstände; aktuelle Website im Browser und per authentifiziertem Abruf ausgewertet |
| Technischer Rahmen | Referenzversionen anhand von Runtime-Dateien, Gemfile.lock und Betriebskonfiguration bestätigt |
| Dokumentverweise | Lokale Markdown-Verweise geprüft; Story- und Epic-Verweise mit tatsächlichen GitHub-Issue-URLs ergänzt |
| Vertrauliche Inhalte | Planung enthält keine Zugangsdaten, privaten Schlüssel, Originalfotos, Datenbanken oder echten Teilnehmerbestände |
| Veröffentlichung | Konzept, Quellen, Design, Architektur, Roadmap, Entscheidungen, Abnahme und sämtliche Storydateien sind auf main veröffentlicht |
| Projektabdeckung | GitHub-Board zeigt 104 Todo-Einträge; Importdialog findet keine weiteren offenen Repository-Issues |
| Gespeicherte Ansichten | Backlog, Umsetzung und Releases sind vorhanden; gespeicherte Einstellungen wurden durch Neuladen geprüft |

## Projektansichten

- [Backlog mit Labels, Meilensteinen und Epic-Bezug](https://github.com/users/marcbey/projects/4/views/1)
- [Umsetzung als Kanbanboard](https://github.com/users/marcbey/projects/4/views/2)
- [Releases nach Meilenstein, gefiltert auf Stories](https://github.com/users/marcbey/projects/4/views/3)

Die Releaseansicht deaktiviert die verschachtelte Hierarchiedarstellung, damit sämtliche Stories in der jeweiligen Releasegruppe gezählt werden. Die nativen Epic-Beziehungen bleiben erhalten.

Die 31 Fachentscheidungen bleiben bewusst offen und benennen benötigte Evidenz, verantwortliche Rolle sowie spätesten Entscheidungspunkt. Sie sind kein Mangel an Planungsabdeckung und dürfen vor Umsetzung des betroffenen Umfangs nicht durch erfundene Fachwerte ersetzt werden.

Es wurden keine Anwendungstests als bestanden ausgegeben: Das Repository enthält derzeit Planung und Vorlagen, noch keine Rails-Produktimplementierung. Die später erforderlichen Fach-, System-, Parallelitäts-, Sicherheits- und Betriebsprüfungen sind je Story und in den Releasegates festgelegt.
