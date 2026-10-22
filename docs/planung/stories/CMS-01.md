# CMS-01 – Redaktionelle Seiten mit Vorschau und Freigabe verwalten

[GitHub-Issue #20](https://github.com/marcbey/the-step-agentic-workflow/issues/20)

## User Story

Als **Redaktion** möchte ich **Redaktionelle Seiten mit Vorschau und Freigabe verwalten**.

**Erwarteter Nutzen:** Vereinsinhalte ohne Codeänderung aktuell zu halten.

## Einordnung

- Story-ID: [CMS-01 #20](https://github.com/marcbey/the-step-agentic-workflow/issues/20) · Epic: [E03 #3](https://github.com/marcbey/the-step-agentic-workflow/issues/3)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: T01, F01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Action Text und Lexxy unterstützen strukturierte Texte innerhalb des Rails-Systems.
- [ ] **AK-02:** Entwurf, Vorschau, Veröffentlichung und Archivierung sind getrennte Zustände.
- [ ] **AK-03:** Nur berechtigte Admins und Editors ändern öffentliche Inhalte.
- [ ] **AK-04:** Slugs bleiben eindeutig; Änderungen erhalten kontrollierte Weiterleitungen.
- [ ] **AK-05:** Systemseiten für Recht und Kontakt bleiben trotz redaktioneller Bearbeitung dauerhaft erreichbar.
- [ ] **AK-06:** Revisionsstand, Bearbeiter und Veröffentlichungszeitpunkt werden nachvollziehbar gespeichert.

## Abhängigkeiten und Voraussetzungen

[BAS-03 #16](https://github.com/marcbey/the-step-agentic-workflow/issues/16), [BAS-05 #18](https://github.com/marcbey/the-step-agentic-workflow/issues/18)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

WebPage und Community-Inhalte mit Action Text/Lexxy; Medien über Active Storage mit geprüften Sichtbarkeitsregeln.

**Voraussichtliche Codeorte:** `app/models/web_page.rb, app/models/community_*.rb, app/controllers/admin/, app/views/community/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Unveröffentlichte Vorschau ohne Berechtigung, konkurrierende Bearbeitung und Script-Eingaben prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
