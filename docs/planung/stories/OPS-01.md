# OPS-01 – Trainereinsätze und Zuständigkeiten planen

[GitHub-Issue #73](https://github.com/marcbey/the-step-agentic-workflow/issues/73)

## User Story

Als **Kurskoordination** möchte ich **Trainereinsätze und Zuständigkeiten planen**.

**Erwarteter Nutzen:** passende Betreuung für alle Termine sicherzustellen.

## Einordnung

- Story-ID: [OPS-01 #73](https://github.com/marcbey/the-step-agentic-workflow/issues/73) · Epic: [E09 #9](https://github.com/marcbey/the-step-agentic-workflow/issues/9)
- Release: **R2** · Priorität: **P0** · vorläufige Größe: **8 Story Points**
- Quelle: F01, F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Aktive Coaches können konkreten Terminen oder definierten Zeiträumen zugeordnet werden.
- [ ] **AK-02:** Übersicht zeigt unbesetzte Termine und erforderliche Betreuungszahl.
- [ ] **AK-03:** Zeitliche Überschneidung und gemeldete Abwesenheit erzeugen Warnung oder Sperre nach festgelegter Regel.
- [ ] **AK-04:** Qualifikationen werden vor der Zuordnung nachvollziehbar geprüft.
- [ ] **AK-05:** Zuordnung allein verleiht keine redaktionellen oder administrativen Rechte.
- [ ] **AK-06:** Änderung und Entzug lösen aktuelle Informationen und sofortige Berechtigungsprüfung aus.

## Abhängigkeiten und Voraussetzungen

[BUC-07 #53](https://github.com/marcbey/the-step-agentic-workflow/issues/53), [BAS-03 #16](https://github.com/marcbey/the-step-agentic-workflow/issues/16)

**Vor Umsetzung zu klären:** D20. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Operative Zugriffskontrolle verwendet aktive Zuordnung und Zeitfenster; Verwaltung und Coach bleiben getrennt.

**Voraussichtliche Codeorte:** `app/models/coach_assignment.rb, app/models/time_entry.rb, app/models/material_item.rb, app/controllers/staff/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Doppelbelegung, inaktiver Coach, ablaufende Qualifikation und später Zuordnungsentzug prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
