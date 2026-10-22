# OPS-06 – Interne News und Mitarbeiterdokumente bereitstellen

[GitHub-Issue #78](https://github.com/marcbey/the-step-agentic-workflow/issues/78)

## User Story

Als **Mitarbeiterin** möchte ich **Interne News und Mitarbeiterdokumente bereitstellen**.

**Erwarteter Nutzen:** aktuelle interne Informationen am richtigen Ort zu finden.

## Einordnung

- Story-ID: [OPS-06 #78](https://github.com/marcbey/the-step-agentic-workflow/issues/78) · Epic: [E09 #9](https://github.com/marcbey/the-step-agentic-workflow/issues/9)
- Release: **R2** · Priorität: **P1** · vorläufige Größe: **5 Story Points**
- Quelle: F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Interne News und Dokumente haben definierte Zielgruppen.
- [ ] **AK-02:** Nur berechtigte Redaktion veröffentlicht interne Inhalte.
- [ ] **AK-03:** Kenntnisnahme kann für ausgewählte Sicherheitsunterlagen angefordert werden.
- [ ] **AK-04:** Abgelaufene Dokumente werden als veraltet gekennzeichnet.
- [ ] **AK-05:** Direktabruf prüft aktiven Zugang und Zielgruppenberechtigung.
- [ ] **AK-06:** Interne Inhalte erscheinen weder in öffentlicher Suche noch öffentlichen Feeds.

## Abhängigkeiten und Voraussetzungen

[BAS-03 #16](https://github.com/marcbey/the-step-agentic-workflow/issues/16), [CMS-01 #20](https://github.com/marcbey/the-step-agentic-workflow/issues/20), [MIT-07 #71](https://github.com/marcbey/the-step-agentic-workflow/issues/71)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Operative Zugriffskontrolle verwendet aktive Zuordnung und Zeitfenster; Verwaltung und Coach bleiben getrennt.

**Voraussichtliche Codeorte:** `app/models/coach_assignment.rb, app/models/time_entry.rb, app/models/material_item.rb, app/controllers/staff/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Öffentliche Suche, deaktivierter Mitarbeiter und Direktdateiabruf aus abgelaufener Sitzung prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
