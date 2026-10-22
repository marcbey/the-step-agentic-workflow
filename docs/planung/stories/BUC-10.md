# BUC-10 – Automatische Erinnerungen zustandsabhängig versenden

[GitHub-Issue #56](https://github.com/marcbey/the-step-agentic-workflow/issues/56)

## User Story

Als **Teilnehmerin** möchte ich **Automatische Erinnerungen zustandsabhängig versenden**.

**Erwarteter Nutzen:** rechtzeitig an den tatsächlich stattfindenden Termin erinnert zu werden.

## Einordnung

- Story-ID: [BUC-10 #56](https://github.com/marcbey/the-step-agentic-workflow/issues/56) · Epic: [E05 #5](https://github.com/marcbey/the-step-agentic-workflow/issues/5)
- Release: **R1** · Priorität: **P1** · vorläufige Größe: **5 Story Points**
- Quelle: F05, T01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Erinnerung wird nach Planungsvorgabe 24 Stunden vor Beginn fällig.
- [ ] **AK-02:** Coach- und Teilnehmererinnerung nutzen getrennte Empfängerregeln.
- [ ] **AK-03:** Versand prüft erneut Buchungs-, Termin- und Zuordnungsstatus.
- [ ] **AK-04:** Verschiebung erzeugt keine Erinnerung zum alten Termin.
- [ ] **AK-05:** Wiederholter Schedulerlauf erzeugt keine neuen Duplikatereignisse.
- [ ] **AK-06:** Ausgefallener Scheduler und überfällige Nachrichten sind im Betrieb erkennbar.

## Abhängigkeiten und Voraussetzungen

[BUC-04 #50](https://github.com/marcbey/the-step-agentic-workflow/issues/50), [BUC-07 #53](https://github.com/marcbey/the-step-agentic-workflow/issues/53)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Booking-Übergang und Outbox in einer Primary-DB-Transaktion; Queueauslieferung ist nachgelagert.

**Voraussichtliche Codeorte:** `app/models/booking.rb, app/services/bookings/, app/controllers/course_bookings_controller.rb, app/jobs/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Terminverschiebung nach Planung, DST-Wechsel, entfernter Coach und mehrfacher Schedulerlauf testen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
