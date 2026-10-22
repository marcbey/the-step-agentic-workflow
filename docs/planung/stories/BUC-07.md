# BUC-07 – Teilnehmerlisten, Check-in und Anwesenheit je Termin führen

[GitHub-Issue #53](https://github.com/marcbey/the-step-agentic-workflow/issues/53)

## User Story

Als **zugeordneter Coach** möchte ich **Teilnehmerlisten, Check-in und Anwesenheit je Termin führen**.

**Erwarteter Nutzen:** den betreuten Termin sicher organisieren zu können.

## Einordnung

- Story-ID: [BUC-07 #53](https://github.com/marcbey/the-step-agentic-workflow/issues/53) · Epic: [E05 #5](https://github.com/marcbey/the-step-agentic-workflow/issues/5)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **8 Story Points**
- Quelle: F01, F04, T01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Liste enthält nur notwendige Daten bestätigter Buchungen.
- [ ] **AK-02:** Coachzugriff besteht ausschließlich für aktive Zuordnung im freigegebenen Zeitfenster.
- [ ] **AK-03:** Anwesend, abwesend, entschuldigt und offen sind je Termin erfassbar.
- [ ] **AK-04:** Mehrtägige Angebote haben getrennte Anwesenheit je Tag.
- [ ] **AK-05:** Änderung, handelnde Person und Zeitpunkt werden nachvollziehbar protokolliert.
- [ ] **AK-06:** Entzug der Zuordnung sperrt Listen, Detail und Export beim nächsten Request.

## Abhängigkeiten und Voraussetzungen

[BUC-02 #26](https://github.com/marcbey/the-step-agentic-workflow/issues/26), [BAS-03 #16](https://github.com/marcbey/the-step-agentic-workflow/issues/16), [ANG-04 #44](https://github.com/marcbey/the-step-agentic-workflow/issues/44)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Booking-Übergang und Outbox in einer Primary-DB-Transaktion; Queueauslieferung ist nachgelagert.

**Voraussichtliche Codeorte:** `app/models/booking.rb, app/services/bookings/, app/controllers/course_bookings_controller.rb, app/jobs/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Fremder Kurs, Zugriff außerhalb sieben Tagen vor/nach dem Termin und paralleler Check-in dürfen keine unzulässigen Änderungen erlauben.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
