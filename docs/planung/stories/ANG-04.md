# ANG-04 – Camps und mehrtägige Workshops als Buchungseinheit führen

[GitHub-Issue #44](https://github.com/marcbey/the-step-agentic-workflow/issues/44)

## User Story

Als **Elternteil** möchte ich **Camps und mehrtägige Workshops als Buchungseinheit führen**.

**Erwarteter Nutzen:** ein Camp mit allen Tagen verlässlich zu buchen.

## Einordnung

- Story-ID: [ANG-04 #44](https://github.com/marcbey/the-step-agentic-workflow/issues/44) · Epic: [E04 #4](https://github.com/marcbey/the-step-agentic-workflow/issues/4)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: F01, F03; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Campdetail zeigt sämtliche Tageszeiten, Orte und Leistungsbestandteile.
- [ ] **AK-02:** Eine Campbuchung belegt genau einen Platz in der gesamten definierten Einheit.
- [ ] **AK-03:** Anwesenheit bleibt je Tag getrennt erfassbar.
- [ ] **AK-04:** Teilnahme an einzelnen Tagen wird nur bei ausdrücklich angebotenem Tagesmodell zugelassen.
- [ ] **AK-05:** Absage oder Verschiebung einzelner Tage informiert alle betroffenen Buchungen.
- [ ] **AK-06:** Kosten und Terminliste werden als historische Buchungssicht gesichert.

## Abhängigkeiten und Voraussetzungen

[ANG-01 #21](https://github.com/marcbey/the-step-agentic-workflow/issues/21), [ANG-02 #22](https://github.com/marcbey/the-step-agentic-workflow/issues/22)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Angebot und einzelne Termine sind getrennt; Serien erzeugen keine zweite öffentliche Kapazitätsquelle.

**Voraussichtliche Codeorte:** `app/models/course_offering.rb, app/models/course_occurrence.rb, app/services/course_series_plan.rb, app/views/courses/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Mehrtägiges Camp mit einem abgesagten Tag und gleichzeitiger Buchung des letzten Platzes testen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
