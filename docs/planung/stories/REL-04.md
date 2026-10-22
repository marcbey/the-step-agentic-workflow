# REL-04 – Releaseabnahme und agentischen Arbeitsablauf festlegen

[GitHub-Issue #95](https://github.com/marcbey/the-step-agentic-workflow/issues/95)

## User Story

Als **Projektverantwortung** möchte ich **Releaseabnahme und agentischen Arbeitsablauf festlegen**.

**Erwarteter Nutzen:** Stories überprüfbar bis zur fachlichen Abnahme zu führen.

## Einordnung

- Story-ID: [REL-04 #95](https://github.com/marcbey/the-step-agentic-workflow/issues/95) · Epic: [E12 #12](https://github.com/marcbey/the-step-agentic-workflow/issues/12)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: T01, F05; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Jede Umsetzung startet aus einer Story mit AKs, Abhängigkeiten und geklärten Blockern.
- [ ] **AK-02:** Ein Branch beziehungsweise PR trägt Story-ID, Nachweis und aktualisierte Dokumentation.
- [ ] **AK-03:** Todo, In Progress und Done unterscheiden Planung, Umsetzung und fachliche Abnahme.
- [ ] **AK-04:** Tests, Sicherheits- und Inhaltsprüfungen sowie echte Konkurrenztests werden pro Risiko verlangt.
- [ ] **AK-05:** Produktivstart benötigt benannte fachliche Abnahme und geprobten Rückfallplan.
- [ ] **AK-06:** R2 und R3 wiederholen die Gates für ihre neuen Datenflüsse und Geschäftsprozesse.

## Abhängigkeiten und Voraussetzungen

[REL-01 #92](https://github.com/marcbey/the-step-agentic-workflow/issues/92), [REL-02 #93](https://github.com/marcbey/the-step-agentic-workflow/issues/93), [REL-03 #94](https://github.com/marcbey/the-step-agentic-workflow/issues/94), [GOV-05 #90](https://github.com/marcbey/the-step-agentic-workflow/issues/90), [GOV-06 #91](https://github.com/marcbey/the-step-agentic-workflow/issues/91)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Runbook und Handbuch folgen dem real implementierten Stand; Produktionsfreigabe ist keine Folge einer Issue-Anlage.

**Voraussichtliche Codeorte:** `docs/deployment.md, docs/runbooks/, app/views/admin/handbook/, .github/workflows/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Abnahmeprotokoll für Eltern-Gastbuchung, Admin-Kursbetrieb und Coach-Check-in; spätere Releases ergänzen Mitgliedschaft und Testkauf.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
