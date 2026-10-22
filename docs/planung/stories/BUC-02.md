# BUC-02 – Plätze atomar reservieren und per E-Mail bestätigen

[GitHub-Issue #26](https://github.com/marcbey/the-step-agentic-workflow/issues/26)

## User Story

Als **buchende Person** möchte ich **Plätze atomar reservieren und per E-Mail bestätigen**.

**Erwarteter Nutzen:** einen Platz ohne Überbuchung zuverlässig zu sichern.

## Einordnung

- Story-ID: [BUC-02 #26](https://github.com/marcbey/the-step-agentic-workflow/issues/26) · Epic: [E05 #5](https://github.com/marcbey/the-step-agentic-workflow/issues/5)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **13 Story Points**
- Quelle: F01, F05, T01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Reservierung gilt höchstens 60 Minuten und endet spätestens mit Kursbeginn.
- [ ] **AK-02:** Freie Plätze sind Kapazität minus bestätigte und noch aktive reservierte Plätze.
- [ ] **AK-03:** Parallele Anfragen auf den letzten Platz erzeugen höchstens eine erfolgreiche Reservierung.
- [ ] **AK-04:** Bestätigungslink ist zweckgebunden und nach Ablauf nicht nutzbar.
- [ ] **AK-05:** Wiederholtes Bestätigen verändert weder Zähler noch Buchung erneut.
- [ ] **AK-06:** Ablauf und Bestätigung werden auch bei konkurrierenden Worker-/Webzugriffen atomar entschieden.

## Abhängigkeiten und Voraussetzungen

[BUC-01 #25](https://github.com/marcbey/the-step-agentic-workflow/issues/25), [BAS-02 #15](https://github.com/marcbey/the-step-agentic-workflow/issues/15)

**Vor Umsetzung zu klären:** D11. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Booking-Übergang und Outbox in einer Primary-DB-Transaktion; Queueauslieferung ist nachgelagert.

**Voraussichtliche Codeorte:** `app/models/booking.rb, app/services/bookings/, app/controllers/course_bookings_controller.rb, app/jobs/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Dateibasiertes SQLite mit getrennten Verbindungen: 20 parallele Anfragen auf einen Platz; Ablauf exakt an der Zeitgrenze; Commitfehler.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
