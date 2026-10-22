# GOV-01 – Einwilligungen, Drittinhalte und Datenschutzeinstellungen trennen

[GitHub-Issue #24](https://github.com/marcbey/the-step-agentic-workflow/issues/24)

## User Story

Als **Besucherin** möchte ich **Einwilligungen, Drittinhalte und Datenschutzeinstellungen trennen**.

**Erwarteter Nutzen:** freiwillige Datenverarbeitung selbst zu steuern.

## Einordnung

- Story-ID: [GOV-01 #24](https://github.com/marcbey/the-step-agentic-workflow/issues/24) · Epic: [E11 #11](https://github.com/marcbey/the-step-agentic-workflow/issues/11)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: F04, W05, T01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Notwendige Websitefunktionen sind von Videos, Karten, Social Feed und Newsletter getrennt.
- [ ] **AK-02:** Optionale Zwecke sind standardmäßig abgelehnt.
- [ ] **AK-03:** Kenntnisnahme eines Buchungshinweises wird nicht als pauschale Einwilligung behandelt.
- [ ] **AK-04:** Einwilligung dokumentiert Zweck, Textversion, Auswahl und Zeitpunkt.
- [ ] **AK-05:** Widerruf ist so leicht erreichbar wie Zustimmung.
- [ ] **AK-06:** Neue optionale Zwecke werden nicht durch frühere pauschale Auswahl freigegeben.

## Abhängigkeiten und Voraussetzungen

[BAS-02 #15](https://github.com/marcbey/the-step-agentic-workflow/issues/15)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Berechtigung pro Request und Datei; separate Retention pro Datenart; keine pauschale Löschung von Finanzbelegen.

**Voraussichtliche Codeorte:** `app/policies/, app/jobs/retention/, config/initializers/, test/security/, test/system/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Neue Consentversion, blockiertes JavaScript und Ablehnen aller Zwecke bei fortgesetzter Buchung prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
