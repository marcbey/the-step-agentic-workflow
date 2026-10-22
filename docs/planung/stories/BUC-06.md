# BUC-06 – Warteliste mit befristetem Nachrückangebot anbieten

[GitHub-Issue #52](https://github.com/marcbey/the-step-agentic-workflow/issues/52)

## User Story

Als **Interessentin** möchte ich **Warteliste mit befristetem Nachrückangebot anbieten**.

**Erwarteter Nutzen:** bei einem vollen Angebot fair nachrücken zu können.

## Einordnung

- Story-ID: [BUC-06 #52](https://github.com/marcbey/the-step-agentic-workflow/issues/52) · Epic: [E05 #5](https://github.com/marcbey/the-step-agentic-workflow/issues/5)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **8 Story Points**
- Quelle: F05; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Nur nicht mehr regulär verfügbare Angebote bieten den Wartelisteneinstieg.
- [ ] **AK-02:** Kontaktbestätigung und eindeutiger Eintrag verhindern unbeabsichtigte Doppelanmeldung.
- [ ] **AK-03:** Nachrücken folgt dokumentierter FIFO-Reihenfolge ohne stille Bevorzugung.
- [ ] **AK-04:** Frei gewordener Platz erzeugt genau ein befristetes Angebot mit 24 Stunden Annahmefrist, gekürzt auf den Buchungsschluss.
- [ ] **AK-05:** Annahme verwendet denselben atomaren Kapazitätsprozess wie eine normale Buchung.
- [ ] **AK-06:** Ablauf, Ablehnung und manueller Eingriff sind nachvollziehbar und bedienen die nächste berechtigte Person.

## Abhängigkeiten und Voraussetzungen

[BUC-02 #26](https://github.com/marcbey/the-step-agentic-workflow/issues/26), [BUC-04 #50](https://github.com/marcbey/the-step-agentic-workflow/issues/50), [BUC-05 #51](https://github.com/marcbey/the-step-agentic-workflow/issues/51)

**Vor Umsetzung zu klären:** D14. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Booking-Übergang und Outbox in einer Primary-DB-Transaktion; Queueauslieferung ist nachgelagert.

**Voraussichtliche Codeorte:** `app/models/booking.rb, app/services/bookings/, app/controllers/course_bookings_controller.rb, app/jobs/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Zwei freie Plätze, gleichzeitiges reguläres Buchen, doppeltes Nachrücken und Ende der Annahmefrist testen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
