# EXT-01 – Spenden und Fördermöglichkeiten anbieten

[GitHub-Issue #96](https://github.com/marcbey/the-step-agentic-workflow/issues/96)

## User Story

Als **unterstützende Person** möchte ich **Spenden und Fördermöglichkeiten anbieten**.

**Erwarteter Nutzen:** den Verein freiwillig finanziell zu fördern.

## Einordnung

- Story-ID: [EXT-01 #96](https://github.com/marcbey/the-step-agentic-workflow/issues/96) · Epic: [E13 #13](https://github.com/marcbey/the-step-agentic-workflow/issues/13)
- Release: **R4** · Priorität: **P2** · vorläufige Größe: **8 Story Points**
- Quelle: F05; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Einmalspende und Fördermitgliedschaft sind verständlich getrennt.
- [ ] **AK-02:** Empfänger, Zweck und Zahlungsweg sind freigegeben.
- [ ] **AK-03:** Zahlung nutzt einen gehosteten freigegebenen Anbieter oder dokumentierte Überweisung.
- [ ] **AK-04:** Spendenbestätigung wird nur entsprechend tatsächlich bestätigter Berechtigung und Zahlung ausgestellt.
- [ ] **AK-05:** Abbruch und doppelte Zahlungsrückmeldung erzeugen keine doppelte Spende.
- [ ] **AK-06:** Buchhaltung und Datenschutz erfassen den Spendenprozess gesondert.

## Abhängigkeiten und Voraussetzungen

[FIN-01 #60](https://github.com/marcbey/the-step-agentic-workflow/issues/60), [FIN-05 #67](https://github.com/marcbey/the-step-agentic-workflow/issues/67), [GOV-02 #59](https://github.com/marcbey/the-step-agentic-workflow/issues/59)

**Vor Umsetzung zu klären:** D27. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Optionale Integration hat einen klaren Anbieter-/Datenvertrag und lässt Kernabläufe bei Ausfall nutzbar.

**Voraussichtliche Codeorte:** `app/services/integrations/, app/controllers/, app/views/, test/contracts/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Anbieter-Sandbox mit Zahlung, Abbruch und doppelt geliefertem Ereignis.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
