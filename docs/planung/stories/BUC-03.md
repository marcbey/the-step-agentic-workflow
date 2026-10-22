# BUC-03 – Preise und Mitgliedervorteile historisch korrekt berechnen

[GitHub-Issue #49](https://github.com/marcbey/the-step-agentic-workflow/issues/49)

## User Story

Als **buchende Person** möchte ich **Preise und Mitgliedervorteile historisch korrekt berechnen**.

**Erwarteter Nutzen:** vor der Bestätigung einen verlässlichen Gesamtbetrag zu sehen.

## Einordnung

- Story-ID: [BUC-03 #49](https://github.com/marcbey/the-step-agentic-workflow/issues/49) · Epic: [E05 #5](https://github.com/marcbey/the-step-agentic-workflow/issues/5)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: F04, F05, T01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Mitglieder- und Nichtmitgliederpreise werden als nichtnegative ganze Cent gespeichert.
- [ ] **AK-02:** Kursgebühr plus Leihgebühr ergibt den serverseitigen Gesamtbetrag.
- [ ] **AK-03:** R1 kennzeichnet selbst angegebene Mitgliedschaft als prüfbedürftig.
- [ ] **AK-04:** Ab R2 nutzt die Berechtigung den wirksamen Mitgliedschaftsstatus statt Browserangaben.
- [ ] **AK-05:** Buchung speichert Preisgruppe, Preisregel und Beträge zum Buchungszeitpunkt.
- [ ] **AK-06:** Spätere Preisänderung verändert keine bereits bestätigte Kostenaufstellung.

## Abhängigkeiten und Voraussetzungen

[BUC-02 #26](https://github.com/marcbey/the-step-agentic-workflow/issues/26)

**Vor Umsetzung zu klären:** D12. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Booking-Übergang und Outbox in einer Primary-DB-Transaktion; Queueauslieferung ist nachgelagert.

**Voraussichtliche Codeorte:** `app/models/booking.rb, app/services/bookings/, app/controllers/course_bookings_controller.rb, app/jobs/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Dezimal-Komma, Preis von 0 Euro, manipulierte Centwerte und nachträgliche Preisänderung prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
