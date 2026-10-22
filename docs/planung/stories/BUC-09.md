# BUC-09 – Kurs- und Wettermitteilungen gezielt versenden

[GitHub-Issue #55](https://github.com/marcbey/the-step-agentic-workflow/issues/55)

## User Story

Als **Kursplanung** möchte ich **Kurs- und Wettermitteilungen gezielt versenden**.

**Erwarteter Nutzen:** Teilnehmende bei Änderungen rechtzeitig zu erreichen.

## Einordnung

- Story-ID: [BUC-09 #55](https://github.com/marcbey/the-step-agentic-workflow/issues/55) · Epic: [E05 #5](https://github.com/marcbey/the-step-agentic-workflow/issues/5)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: F02, F05, T01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Terminänderung, Ausfall und Regenersatz besitzen getrennte Nachrichtentypen.
- [ ] **AK-02:** Empfänger werden vor dem Versand als Anzahl und Auswahlgrund angezeigt.
- [ ] **AK-03:** Es werden nur aktuell betroffene bestätigte Kontakte angeschrieben.
- [ ] **AK-04:** Keine Empfängeradresse wird anderen Teilnehmenden offengelegt.
- [ ] **AK-05:** Nachrichten und Ergebnisstatus sind minimiert nachvollziehbar.
- [ ] **AK-06:** Die Kursentscheidung stammt von Berechtigten und wird nicht automatisch aus einer Wetteranzeige abgeleitet.

## Abhängigkeiten und Voraussetzungen

[BUC-04 #50](https://github.com/marcbey/the-step-agentic-workflow/issues/50), [BUC-07 #53](https://github.com/marcbey/the-step-agentic-workflow/issues/53)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Booking-Übergang und Outbox in einer Primary-DB-Transaktion; Queueauslieferung ist nachgelagert.

**Voraussichtliche Codeorte:** `app/models/booking.rb, app/services/bookings/, app/controllers/course_bookings_controller.rb, app/jobs/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Abgesagte, umgebuchte und anonymisierte Kontakte kurz vor Versand erneut prüfen; Mailausfall wiederholen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
