# EXT-07 – Skateparks in Stuttgart als Übersicht bereitstellen

[GitHub-Issue #102](https://github.com/marcbey/the-step-agentic-workflow/issues/102)

## User Story

Als **Skaterin** möchte ich **Skateparks in Stuttgart als Übersicht bereitstellen**.

**Erwarteter Nutzen:** passende Orte mit klaren Nutzungsinformationen zu finden.

## Einordnung

- Story-ID: [EXT-07 #102](https://github.com/marcbey/the-step-agentic-workflow/issues/102) · Epic: [E13 #13](https://github.com/marcbey/the-step-agentic-workflow/issues/13)
- Release: **R4** · Priorität: **P2** · vorläufige Größe: **5 Story Points**
- Quelle: F05; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Einträge enthalten bestätigten Namen, Ort und Art des Skateparks.
- [ ] **AK-02:** Zugänglichkeit, Regeln und Quellen haben ein Prüfdatum.
- [ ] **AK-03:** Karte ist optional und besitzt eine nutzbare Listenalternative.
- [ ] **AK-04:** Stuttpark und Vereinsangebote bleiben in ihrer Verantwortung getrennt.
- [ ] **AK-05:** Verein behauptet keine Betreiberzuständigkeit für fremde Orte.
- [ ] **AK-06:** Fehlerhafte oder veraltete Angaben können gemeldet und redaktionell korrigiert werden.

## Abhängigkeiten und Voraussetzungen

[WEB-05 #36](https://github.com/marcbey/the-step-agentic-workflow/issues/36), [CMS-01 #20](https://github.com/marcbey/the-step-agentic-workflow/issues/20)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Optionale Integration hat einen klaren Anbieter-/Datenvertrag und lässt Kernabläufe bei Ausfall nutzbar.

**Voraussichtliche Codeorte:** `app/services/integrations/, app/controllers/, app/views/, test/contracts/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Geschlossener Park, verweigerte Kartenzustimmung und fehlende Standortdaten prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
