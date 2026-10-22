# BUC-08 – Manuelle Buchungen und sichere Exporte ermöglichen

[GitHub-Issue #54](https://github.com/marcbey/the-step-agentic-workflow/issues/54)

## User Story

Als **Verwaltung** möchte ich **Manuelle Buchungen und sichere Exporte ermöglichen**.

**Erwarteter Nutzen:** Telefonanmeldungen und benötigte Teilnehmerdaten konsistent zu bearbeiten.

## Einordnung

- Story-ID: [BUC-08 #54](https://github.com/marcbey/the-step-agentic-workflow/issues/54) · Epic: [E05 #5](https://github.com/marcbey/the-step-agentic-workflow/issues/5)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: F01, F04, T01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Manuelle Anmeldung verwendet dieselben Kapazitäts- und Preisregeln.
- [ ] **AK-02:** Direktbestätigung durch berechtigte Verwaltung ist als manuell protokolliert.
- [ ] **AK-03:** Filter nach Termin, Status und notwendigem Teilnehmermerkmal sind kombinierbar.
- [ ] **AK-04:** CSV-Export erfordert explizite berechtigte Aktion und schützt vor Tabellenformeln.
- [ ] **AK-05:** Export enthält keine Tokens und keine sensiblen Freitexte.
- [ ] **AK-06:** Anonymisierte Buchungen und nicht mehr berechtigte Kurse bleiben ausgeschlossen.

## Abhängigkeiten und Voraussetzungen

[BUC-02 #26](https://github.com/marcbey/the-step-agentic-workflow/issues/26), [BUC-03 #49](https://github.com/marcbey/the-step-agentic-workflow/issues/49), [BUC-07 #53](https://github.com/marcbey/the-step-agentic-workflow/issues/53)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Booking-Übergang und Outbox in einer Primary-DB-Transaktion; Queueauslieferung ist nachgelagert.

**Voraussichtliche Codeorte:** `app/models/booking.rb, app/services/bookings/, app/controllers/course_bookings_controller.rb, app/jobs/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Telefonbuchung parallel zur Gastbuchung, CSV mit =-Präfix und Exportzugriff nach Rollenentzug prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
