# EVT-01 – Veranstaltungskalender und Eventdetails veröffentlichen

[GitHub-Issue #30](https://github.com/marcbey/the-step-agentic-workflow/issues/30)

## User Story

Als **Communitymitglied** möchte ich **Veranstaltungskalender und Eventdetails veröffentlichen**.

**Erwarteter Nutzen:** Contests und Vereinsveranstaltungen zu planen.

## Einordnung

- Story-ID: [EVT-01 #30](https://github.com/marcbey/the-step-agentic-workflow/issues/30) · Epic: [E06 #6](https://github.com/marcbey/the-step-agentic-workflow/issues/6)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: F01, F03, F05; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Landesmeisterschaften, Contests, Jam Sessions, School’s Out und Ferienprogramme sind kategorisierbar.
- [ ] **AK-02:** Liste und Kalender zeigen Datum, Ort, Veranstalter und Status.
- [ ] **AK-03:** Mehrtagestermine bleiben auf Mobilgeräten verständlich.
- [ ] **AK-04:** Vergangene Events wechseln in ein Archiv und gelten nicht als nächste Veranstaltung.
- [ ] **AK-05:** Absage und Verschiebung werden in Liste, Detail und Startseite konsistent angezeigt.
- [ ] **AK-06:** Kalenderexport enthält nur öffentliche Daten und aktualisierbare Eventkennungen.

## Abhängigkeiten und Voraussetzungen

[CMS-01 #20](https://github.com/marcbey/the-step-agentic-workflow/issues/20), [ANG-02 #22](https://github.com/marcbey/the-step-agentic-workflow/issues/22)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Eventanmeldung verwendet Booking; allgemeine Anfrage erzeugt ohne Prüfung keine Buchungsbestätigung.

**Voraussichtliche Codeorte:** `app/models/community_event.rb, app/models/contact_request.rb, app/mailers/, app/jobs/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Mehrtagesevent, abgesagten Contest, Jahreswechsel und leeren Monat prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
