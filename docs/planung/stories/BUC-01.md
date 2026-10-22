# BUC-01 – Gastbuchung mit Minderjährigen- und Einwilligungslogik anbieten

[GitHub-Issue #25](https://github.com/marcbey/the-step-agentic-workflow/issues/25)

## User Story

Als **Elternteil** möchte ich **Gastbuchung mit Minderjährigen- und Einwilligungslogik anbieten**.

**Erwarteter Nutzen:** ein Kind ohne erzwungenes Benutzerkonto anzumelden.

## Einordnung

- Story-ID: [BUC-01 #25](https://github.com/marcbey/the-step-agentic-workflow/issues/25) · Epic: [E05 #5](https://github.com/marcbey/the-step-agentic-workflow/issues/5)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **8 Story Points**
- Quelle: F01, F04, T01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Buchung erfasst die laut Angebotskonfiguration notwendigen Teilnehmer- und Kontaktdaten.
- [ ] **AK-02:** Alter wird am tatsächlichen Angebotsbeginn berechnet.
- [ ] **AK-03:** Unter 18 Jahren sind Name und Telefonnummer einer erziehungsberechtigten Person erforderlich.
- [ ] **AK-04:** Datenschutzhinweis wird als Kenntnisnahme mit Version dokumentiert.
- [ ] **AK-05:** Optionales sensibles Freitextfeld ist standardmäßig aus und benötigt gesonderte freigegebene Einwilligung.
- [ ] **AK-06:** Ungültige Eingabe erhält Feldfehler ohne unnötigen Verlust bereits erfasster Daten.

## Abhängigkeiten und Voraussetzungen

[ANG-01 #21](https://github.com/marcbey/the-step-agentic-workflow/issues/21), [ANG-07 #23](https://github.com/marcbey/the-step-agentic-workflow/issues/23), [GOV-01 #24](https://github.com/marcbey/the-step-agentic-workflow/issues/24)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Booking-Übergang und Outbox in einer Primary-DB-Transaktion; Queueauslieferung ist nachgelagert.

**Voraussichtliche Codeorte:** `app/models/booking.rb, app/services/bookings/, app/controllers/course_bookings_controller.rb, app/jobs/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Person wird am Kurstag 18, falsches Geburtsdatum, fehlende Elternangabe und abgelehnte optionale Einwilligung prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
