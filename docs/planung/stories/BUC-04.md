# BUC-04 – Buchungse-Mails und Versandwiederholung zuverlässig ausliefern

[GitHub-Issue #50](https://github.com/marcbey/the-step-agentic-workflow/issues/50)

## User Story

Als **buchende Person** möchte ich **Buchungse-Mails und Versandwiederholung zuverlässig ausliefern**.

**Erwarteter Nutzen:** Status, Termine und Kosten auch nach einem Mailfehler zu erhalten.

## Einordnung

- Story-ID: [BUC-04 #50](https://github.com/marcbey/the-step-agentic-workflow/issues/50) · Epic: [E05 #5](https://github.com/marcbey/the-step-agentic-workflow/issues/5)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **8 Story Points**
- Quelle: F01, F05, T01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Reservierung, Bestätigung, Ablauf und Storno verwenden klar unterscheidbare Texte.
- [ ] **AK-02:** Dauerhafte Outbox entsteht in derselben Transaktion wie die fachliche Änderung.
- [ ] **AK-03:** Solid Queue verarbeitet und wiederholt fehlgeschlagene Auslieferungen.
- [ ] **AK-04:** Eindeutiger Ereignisschlüssel verhindert mehrfach erzeugte fachliche Benachrichtigungen.
- [ ] **AK-05:** Admin erkennt fehlgeschlagene Zustellung und kann berechtigt erneut auslösen.
- [ ] **AK-06:** Empfängerdaten und Tokens werden weder in Logmeldungen noch offenen Auditdetails ausgegeben.

## Abhängigkeiten und Voraussetzungen

[BUC-02 #26](https://github.com/marcbey/the-step-agentic-workflow/issues/26), [BAS-04 #17](https://github.com/marcbey/the-step-agentic-workflow/issues/17)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Booking-Übergang und Outbox in einer Primary-DB-Transaktion; Queueauslieferung ist nachgelagert.

**Voraussichtliche Codeorte:** `app/models/booking.rb, app/services/bookings/, app/controllers/course_bookings_controller.rb, app/jobs/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** SMTP-Timeout nach Annahme, Workerabbruch und Wiederholung simulieren; mögliche Transportdubletten fachlich schadlos halten.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
