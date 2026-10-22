# OPS-07 – Materialbestand, Ausgabe und Wartung verwalten

[GitHub-Issue #79](https://github.com/marcbey/the-step-agentic-workflow/issues/79)

## User Story

Als **Materialkoordination** möchte ich **Materialbestand, Ausgabe und Wartung verwalten**.

**Erwarteter Nutzen:** Leihmaterial einsatzfähig und verfügbar zu halten.

## Einordnung

- Story-ID: [OPS-07 #79](https://github.com/marcbey/the-step-agentic-workflow/issues/79) · Epic: [E09 #9](https://github.com/marcbey/the-step-agentic-workflow/issues/9)
- Release: **R2** · Priorität: **P1** · vorläufige Größe: **8 Story Points**
- Quelle: F02, F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Bestand unterscheidet Boards, Helme und Schutzausrüstung nach notwendiger Größe.
- [ ] **AK-02:** Verfügbar, ausgeliehen, defekt und in Wartung sind getrennte Zustände.
- [ ] **AK-03:** Ausgabe und Rückgabe werden einem Termin oder Vorgang zugeordnet.
- [ ] **AK-04:** Defektes Material zählt nicht zur verfügbaren Ausstattung.
- [ ] **AK-05:** Offener Leihbedarf ist aus Buchungen aggregiert sichtbar.
- [ ] **AK-06:** Korrekturen und Verlust werden nachvollziehbar protokolliert.

## Abhängigkeiten und Voraussetzungen

[ANG-07 #23](https://github.com/marcbey/the-step-agentic-workflow/issues/23), [BUC-07 #53](https://github.com/marcbey/the-step-agentic-workflow/issues/53)

**Vor Umsetzung zu klären:** D22. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Operative Zugriffskontrolle verwendet aktive Zuordnung und Zeitfenster; Verwaltung und Coach bleiben getrennt.

**Voraussichtliche Codeorte:** `app/models/coach_assignment.rb, app/models/time_entry.rb, app/models/material_item.rb, app/controllers/staff/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Gleichzeitige Ausgabe des letzten Helms, defektes Board und verspätete Rückgabe prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
