# OPS-02 – Persönlichen Mitarbeiterkalender und Kursbesetzung anzeigen

[GitHub-Issue #74](https://github.com/marcbey/the-step-agentic-workflow/issues/74)

## User Story

Als **Mitarbeiterin** möchte ich **Persönlichen Mitarbeiterkalender und Kursbesetzung anzeigen**.

**Erwarteter Nutzen:** die eigenen Einsätze und freigegebenen Aufgaben zu überblicken.

## Einordnung

- Story-ID: [OPS-02 #74](https://github.com/marcbey/the-step-agentic-workflow/issues/74) · Epic: [E09 #9](https://github.com/marcbey/the-step-agentic-workflow/issues/9)
- Release: **R2** · Priorität: **P1** · vorläufige Größe: **5 Story Points**
- Quelle: F01, F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Mein Kalender zeigt wirksame Einsätze mit Zeit, Ort und Status.
- [ ] **AK-02:** Kursbesetzungsliste zeigt nur im eigenen Aufgabenbereich notwendige Personaldaten.
- [ ] **AK-03:** Direkter Teilnehmerzugriff folgt weiterhin den zeitlichen Coachregeln.
- [ ] **AK-04:** Absagen und Vertretungen werden ohne veraltete Zusagen dargestellt.
- [ ] **AK-05:** Persönlicher Kalenderexport enthält keine Teilnehmer- oder Kinderdaten.
- [ ] **AK-06:** Leerer Kalender und kollidierende Termine erhalten verständliche Hinweise.

## Abhängigkeiten und Voraussetzungen

[OPS-01 #73](https://github.com/marcbey/the-step-agentic-workflow/issues/73)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Operative Zugriffskontrolle verwendet aktive Zuordnung und Zeitfenster; Verwaltung und Coach bleiben getrennt.

**Voraussichtliche Codeorte:** `app/models/coach_assignment.rb, app/models/time_entry.rb, app/models/material_item.rb, app/controllers/staff/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Zuweisung entfernen und vorhandenen Kalenderlink erneut laden; Export auf personenbezogene Kursdaten prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
