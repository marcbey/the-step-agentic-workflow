# ANG-03 – Angebotsübersicht und Angebotsdetails bereitstellen

[GitHub-Issue #27](https://github.com/marcbey/the-step-agentic-workflow/issues/27)

## User Story

Als **buchende Person** möchte ich **Angebotsübersicht und Angebotsdetails bereitstellen**.

**Erwarteter Nutzen:** ein passendes Angebot nach Alter, Level und Termin zu finden.

## Einordnung

- Story-ID: [ANG-03 #27](https://github.com/marcbey/the-step-agentic-workflow/issues/27) · Epic: [E04 #4](https://github.com/marcbey/the-step-agentic-workflow/issues/4)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: F03, F05; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Filter unterstützen Angebotsart, Altersgruppe, Level und Zeitraum.
- [ ] **AK-02:** Detailseite zeigt Ort, alle Termine, Kosten, Leihoptionen und Mitbringliste.
- [ ] **AK-03:** Freie Plätze berücksichtigen bestätigte Buchungen und aktive Reservierungen.
- [ ] **AK-04:** Buchungsschluss und Absagezustand werden mit Text erklärt.
- [ ] **AK-05:** Gefilterte Ansichten sind verlinkbar und behalten Auswahl bei der Rückkehr.
- [ ] **AK-06:** Ohne JavaScript bleiben Informationen und primärer Buchungsweg nutzbar.

## Abhängigkeiten und Voraussetzungen

[ANG-01 #21](https://github.com/marcbey/the-step-agentic-workflow/issues/21), [ANG-02 #22](https://github.com/marcbey/the-step-agentic-workflow/issues/22), [BUC-02 #26](https://github.com/marcbey/the-step-agentic-workflow/issues/26)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Angebot und einzelne Termine sind getrennt; Serien erzeugen keine zweite öffentliche Kapazitätsquelle.

**Voraussichtliche Codeorte:** `app/models/course_offering.rb, app/models/course_occurrence.rb, app/services/course_series_plan.rb, app/views/courses/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Filter ohne Treffer, gerade ausgebuchtes Angebot und mehrtägigen Camptermin prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
