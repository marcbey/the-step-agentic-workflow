# OPS-05 – Abwesenheit, Urlaub und Vertretung bearbeiten

[GitHub-Issue #77](https://github.com/marcbey/the-step-agentic-workflow/issues/77)

## User Story

Als **Mitarbeiterin** möchte ich **Abwesenheit, Urlaub und Vertretung bearbeiten**.

**Erwarteter Nutzen:** Verhinderung frühzeitig mit der Einsatzplanung abzustimmen.

## Einordnung

- Story-ID: [OPS-05 #77](https://github.com/marcbey/the-step-agentic-workflow/issues/77) · Epic: [E09 #9](https://github.com/marcbey/the-step-agentic-workflow/issues/9)
- Release: **R2** · Priorität: **P1** · vorläufige Größe: **5 Story Points**
- Quelle: F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Abwesenheit wird mit Zeitraum und notwendiger Kategorie beantragt.
- [ ] **AK-02:** Private Begründung wird nicht allen Kollegen angezeigt.
- [ ] **AK-03:** Prüfung zeigt betroffene bestätigte Einsätze.
- [ ] **AK-04:** Genehmigung entfernt keine Betreuung ohne geregelte Vertretung oder offene Warnung.
- [ ] **AK-05:** Vertretung muss aktiv und fachlich berechtigt sein.
- [ ] **AK-06:** Betroffene Coaches und Koordination erhalten eine konsistente Änderungsmitteilung.

## Abhängigkeiten und Voraussetzungen

[OPS-01 #73](https://github.com/marcbey/the-step-agentic-workflow/issues/73), [OPS-02 #74](https://github.com/marcbey/the-step-agentic-workflow/issues/74)

**Vor Umsetzung zu klären:** D20. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Operative Zugriffskontrolle verwendet aktive Zuordnung und Zeitfenster; Verwaltung und Coach bleiben getrennt.

**Voraussichtliche Codeorte:** `app/models/coach_assignment.rb, app/models/time_entry.rb, app/models/material_item.rb, app/controllers/staff/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Teilüberlappender Urlaub, kurzfristige Verhinderung und unqualifizierte Vertretung prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
