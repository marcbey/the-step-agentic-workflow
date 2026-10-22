# GOV-04 – Auskunft, Berichtigung, Widerruf und Löschung bearbeiten

[GitHub-Issue #89](https://github.com/marcbey/the-step-agentic-workflow/issues/89)

## User Story

Als **betroffene Person** möchte ich **Auskunft, Berichtigung, Widerruf und Löschung bearbeiten**.

**Erwarteter Nutzen:** die eigenen Daten nachvollziehbar verwalten zu lassen.

## Einordnung

- Story-ID: [GOV-04 #89](https://github.com/marcbey/the-step-agentic-workflow/issues/89) · Epic: [E11 #11](https://github.com/marcbey/the-step-agentic-workflow/issues/11)
- Release: **R2** · Priorität: **P1** · vorläufige Größe: **8 Story Points**
- Quelle: F02, F04, W05; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Anfrage wird nach geeignetem Identitätsnachweis der richtigen Person zugeordnet.
- [ ] **AK-02:** Auskunft erfasst alle freigegebenen fachlichen Bereiche ohne fremde Familiendaten.
- [ ] **AK-03:** Berichtigung verändert keine bereits ausgestellten Belege stillschweigend.
- [ ] **AK-04:** Widerruf optionaler Gesundheitsangaben leert das Feld ohne automatische Kursstornierung.
- [ ] **AK-05:** Löschung berücksichtigt getrennte gesetzlich oder fachlich bestätigte Aufbewahrungspflichten.
- [ ] **AK-06:** Erledigung und eingeschränkte Ausnahmen werden ohne sensible Inhaltskopien dokumentiert.

## Abhängigkeiten und Voraussetzungen

[GOV-03 #88](https://github.com/marcbey/the-step-agentic-workflow/issues/88), [MIT-06 #65](https://github.com/marcbey/the-step-agentic-workflow/issues/65)

**Vor Umsetzung zu klären:** D25. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Berechtigung pro Request und Datei; separate Retention pro Datenart; keine pauschale Löschung von Finanzbelegen.

**Voraussichtliche Codeorte:** `app/policies/, app/jobs/retention/, config/initializers/, test/security/, test/system/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Person mit Gastbuchung und Mitgliedskonto, verwechslungsfähiger Name und zurückgenommene Familienfreigabe prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
