# OPS-03 – Arbeits- und Ehrenamtsstunden erfassen

[GitHub-Issue #75](https://github.com/marcbey/the-step-agentic-workflow/issues/75)

## User Story

Als **Mitarbeiterin** möchte ich **Arbeits- und Ehrenamtsstunden erfassen**.

**Erwarteter Nutzen:** geleistete Zeit nachvollziehbar einzureichen.

## Einordnung

- Story-ID: [OPS-03 #75](https://github.com/marcbey/the-step-agentic-workflow/issues/75) · Epic: [E09 #9](https://github.com/marcbey/the-step-agentic-workflow/issues/9)
- Release: **R2** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: F01, F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Eintrag enthält Datum, Beginn, Ende, Pause und Tätigkeit.
- [ ] **AK-02:** Bezug zu einem Einsatz ist optional und prüfbar.
- [ ] **AK-03:** Negative Dauer, Pause über Gesamtdauer und doppelte Zeiträume werden abgewiesen.
- [ ] **AK-04:** Entwurf und eingereicht sind getrennte Zustände.
- [ ] **AK-05:** Mitarbeitende bearbeiten nur eigene noch nicht freigegebene Einträge.
- [ ] **AK-06:** Zeitberechnung behandelt Mitternacht und Zeitumstellung gemäß dokumentierter Regel.

## Abhängigkeiten und Voraussetzungen

[BAS-03 #16](https://github.com/marcbey/the-step-agentic-workflow/issues/16), [OPS-01 #73](https://github.com/marcbey/the-step-agentic-workflow/issues/73)

**Vor Umsetzung zu klären:** D21. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Operative Zugriffskontrolle verwendet aktive Zuordnung und Zeitfenster; Verwaltung und Coach bleiben getrennt.

**Voraussichtliche Codeorte:** `app/models/coach_assignment.rb, app/models/time_entry.rb, app/models/material_item.rb, app/controllers/staff/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Über-Mitternacht-Eintrag, DST-Wechsel, überlappende Tätigkeiten und fremde User-ID prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
