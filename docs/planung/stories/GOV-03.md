# GOV-03 – Datenaufbewahrung und automatische Bereinigung umsetzen

[GitHub-Issue #88](https://github.com/marcbey/the-step-agentic-workflow/issues/88)

## User Story

Als **Datenschutzverantwortung** möchte ich **Datenaufbewahrung und automatische Bereinigung umsetzen**.

**Erwarteter Nutzen:** Daten nur so lange wie freigegeben zu speichern.

## Einordnung

- Story-ID: [GOV-03 #88](https://github.com/marcbey/the-step-agentic-workflow/issues/88) · Epic: [E11 #11](https://github.com/marcbey/the-step-agentic-workflow/issues/11)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **8 Story Points**
- Quelle: T01, W05; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Referenzfristen für Buchungen sind als technische Ausgangsbasis dokumentiert und fachlich zu bestätigen.
- [ ] **AK-02:** Abgelaufene unbestätigte Anfragen werden nach 24 Stunden gelöscht.
- [ ] **AK-03:** Sensibles Sonstiges wird 30 Tage nach Angebotsende entfernt; übrige direkte Buchungsdaten nach 90 Tagen anonymisiert.
- [ ] **AK-04:** Mitgliedschaft, Stunden und Belege besitzen eigene bestätigte Fristen.
- [ ] **AK-05:** Bereinigung von Details, Audit und Statistik erfolgt konsistent und wiederholbar.
- [ ] **AK-06:** Backups haben eigenen Lebenszyklus; Restore führt Retention vor weiterer Nutzung erneut aus.

## Abhängigkeiten und Voraussetzungen

[BUC-02 #26](https://github.com/marcbey/the-step-agentic-workflow/issues/26), [BUC-07 #53](https://github.com/marcbey/the-step-agentic-workflow/issues/53), [BAS-04 #17](https://github.com/marcbey/the-step-agentic-workflow/issues/17)

**Vor Umsetzung zu klären:** D25. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Berechtigung pro Request und Datei; separate Retention pro Datenart; keine pauschale Löschung von Finanzbelegen.

**Voraussichtliche Codeorte:** `app/policies/, app/jobs/retention/, config/initializers/, test/security/, test/system/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Grenzzeitpunkte, Jobabbruch nach Teilschritt, wiederholter Lauf und Restore vorsehen; spätere Kurse dürfen nicht mitgelöscht werden.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
