# MIT-04 – Kündigungen und Mitgliedschaftswechsel abwickeln

[GitHub-Issue #69](https://github.com/marcbey/the-step-agentic-workflow/issues/69)

## User Story

Als **Mitglied** möchte ich **Kündigungen und Mitgliedschaftswechsel abwickeln**.

**Erwarteter Nutzen:** eine Änderung mit verlässlichem Wirksamkeitsdatum einzureichen.

## Einordnung

- Story-ID: [MIT-04 #69](https://github.com/marcbey/the-step-agentic-workflow/issues/69) · Epic: [E08 #8](https://github.com/marcbey/the-step-agentic-workflow/issues/8)
- Release: **R2** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: F02; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Kündigungsanfrage nennt Eingang und berechnetes vorgesehenes Enddatum.
- [ ] **AK-02:** Fristen folgen der wirksamen Ordnung statt hart codierter Annahmen.
- [ ] **AK-03:** Ausnahmeentscheidung ist berechtigt, begründet und protokolliert.
- [ ] **AK-04:** Wirksamkeit beendet Vorteile und künftige Beitragsforderungen zum richtigen Zeitpunkt.
- [ ] **AK-05:** Bestehende Buchungen und ausgestellte Belege werden nicht stillschweigend gelöscht.
- [ ] **AK-06:** Mitglied erhält nachvollziehbare Bestätigung und Kontaktweg für Rückfragen.

## Abhängigkeiten und Voraussetzungen

[MIT-02 #63](https://github.com/marcbey/the-step-agentic-workflow/issues/63), [FIN-03 #64](https://github.com/marcbey/the-step-agentic-workflow/issues/64)

**Vor Umsetzung zu klären:** D17. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

User bezeichnet Zugang; Membership den Mitgliedschaftsstatus; Kind/Teilnehmer erhält nicht automatisch ein Login.

**Voraussichtliche Codeorte:** `app/models/membership.rb, app/models/guardian_relationship.rb, app/controllers/portal/, app/services/memberships/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Kündigung an der Fristgrenze, spätere Rücknahme und erneuter Periodenlauf prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
