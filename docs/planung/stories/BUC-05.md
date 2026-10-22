# BUC-05 – Selbststorno, Umbuchung und Angebotsabsage durchführen

[GitHub-Issue #51](https://github.com/marcbey/the-step-agentic-workflow/issues/51)

## User Story

Als **buchende Person** möchte ich **Selbststorno, Umbuchung und Angebotsabsage durchführen**.

**Erwarteter Nutzen:** eine Buchung gemäß den bekannten Regeln ändern zu können.

## Einordnung

- Story-ID: [BUC-05 #51](https://github.com/marcbey/the-step-agentic-workflow/issues/51) · Epic: [E05 #5](https://github.com/marcbey/the-step-agentic-workflow/issues/5)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **8 Story Points**
- Quelle: F04, F05, T01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Sicherer Stornolink zeigt vor Ausführung die betroffene Buchung.
- [ ] **AK-02:** Zulässige Frist und mögliche Kosten sind vor Bestätigung sichtbar.
- [ ] **AK-03:** Storno gibt den Platz atomar frei und erzeugt eine nachvollziehbare Aktion.
- [ ] **AK-04:** Umbuchung prüft Zielkapazität und hält Ursprung bei Fehlschlag unverändert.
- [ ] **AK-05:** Angebotsabsage informiert bestätigte und wartende Personen ohne neue Zusage.
- [ ] **AK-06:** Finanzielle Korrekturen folgen einem eigenen Belegprozess und überschreiben keine Rechnung.

## Abhängigkeiten und Voraussetzungen

[BUC-02 #26](https://github.com/marcbey/the-step-agentic-workflow/issues/26), [BUC-04 #50](https://github.com/marcbey/the-step-agentic-workflow/issues/50)

**Vor Umsetzung zu klären:** D13. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Booking-Übergang und Outbox in einer Primary-DB-Transaktion; Queueauslieferung ist nachgelagert.

**Voraussichtliche Codeorte:** `app/models/booking.rb, app/services/bookings/, app/controllers/course_bookings_controller.rb, app/jobs/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Doppelstorno, parallele Umbuchung auf den letzten Platz und abgelaufenen Link prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
