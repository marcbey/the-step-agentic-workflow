# EXT-06 – Mitglieder werben Mitglieder kontrolliert anbieten

[GitHub-Issue #101](https://github.com/marcbey/the-step-agentic-workflow/issues/101)

## User Story

Als **Mitglied** möchte ich **Mitglieder werben Mitglieder kontrolliert anbieten**.

**Erwarteter Nutzen:** eine beschlossene Empfehlungsvorteilsregel zu nutzen.

## Einordnung

- Story-ID: [EXT-06 #101](https://github.com/marcbey/the-step-agentic-workflow/issues/101) · Epic: [E13 #13](https://github.com/marcbey/the-step-agentic-workflow/issues/13)
- Release: **R4** · Priorität: **P2** · vorläufige Größe: **5 Story Points**
- Quelle: F05; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Vorstand legt Berechtigung, Vorteil, Zeitraum und Obergrenze fest.
- [ ] **AK-02:** Empfehlungscode enthält keine offen lesbaren Mitgliedsdaten.
- [ ] **AK-03:** Vorteil entsteht erst nach bestätigter berechtigter Neuaufnahme.
- [ ] **AK-04:** Selbstempfehlung und mehrfache Gewährung für dieselbe Person sind gesperrt.
- [ ] **AK-05:** Kündigung oder Ablehnung folgt einer dokumentierten Rücknahmeregel.
- [ ] **AK-06:** Einladung übermittelt keine fremde Kontaktadresse ohne selbst ausgelösten Vorgang.

## Abhängigkeiten und Voraussetzungen

[MIT-02 #63](https://github.com/marcbey/the-step-agentic-workflow/issues/63), [MIT-05 #70](https://github.com/marcbey/the-step-agentic-workflow/issues/70)

**Vor Umsetzung zu klären:** D30. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Optionale Integration hat einen klaren Anbieter-/Datenvertrag und lässt Kernabläufe bei Ausfall nutzbar.

**Voraussichtliche Codeorte:** `app/services/integrations/, app/controllers/, app/views/, test/contracts/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Selbstwerbung, zwei werbende Personen und abgelehnten Mitgliedsantrag prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
