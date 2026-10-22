# ANG-02 – Serien, Ausnahmen und Ferien im Kurskalender planen

[GitHub-Issue #22](https://github.com/marcbey/the-step-agentic-workflow/issues/22)

## User Story

Als **Kursplanung** möchte ich **Serien, Ausnahmen und Ferien im Kurskalender planen**.

**Erwarteter Nutzen:** regelmäßige Termine ohne versehentliche Ferienbuchung zu organisieren.

## Einordnung

- Story-ID: [ANG-02 #22](https://github.com/marcbey/the-step-agentic-workflow/issues/22) · Epic: [E04 #4](https://github.com/marcbey/the-step-agentic-workflow/issues/4)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **8 Story Points**
- Quelle: F03, T01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Serien erzeugen nachvollziehbare einzelne Termine in Europe/Berlin.
- [ ] **AK-02:** Ferien und Feiertage verwenden versionierte amtliche BW-Quelldaten.
- [ ] **AK-03:** Ausnahme, Ersatztermin und Absage überschreiben nur den gewählten Termin.
- [ ] **AK-04:** Änderungen einer Serie zeigen vorab ihre Wirkung auf bestehende Buchungen.
- [ ] **AK-05:** Doppelte Termine werden bei erneutem Generierungslauf verhindert.
- [ ] **AK-06:** Vergangene Termine können nicht stillschweigend umgeplant werden.

## Abhängigkeiten und Voraussetzungen

[ANG-01 #21](https://github.com/marcbey/the-step-agentic-workflow/issues/21)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Angebot und einzelne Termine sind getrennt; Serien erzeugen keine zweite öffentliche Kapazitätsquelle.

**Voraussichtliche Codeorte:** `app/models/course_offering.rb, app/models/course_occurrence.rb, app/services/course_series_plan.rb, app/views/courses/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Sommer-/Winterzeitwechsel, Schulferien, Serienänderung und doppelten Generierungslauf testen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
