# MIT-05 – Mitgliedervorteile zentral und zeitabhängig prüfen

[GitHub-Issue #70](https://github.com/marcbey/the-step-agentic-workflow/issues/70)

## User Story

Als **Mitglied** möchte ich **Mitgliedervorteile zentral und zeitabhängig prüfen**.

**Erwarteter Nutzen:** berechtigte Vergünstigungen automatisch zu erhalten.

## Einordnung

- Story-ID: [MIT-05 #70](https://github.com/marcbey/the-step-agentic-workflow/issues/70) · Epic: [E08 #8](https://github.com/marcbey/the-step-agentic-workflow/issues/8)
- Release: **R2** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: F01, F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Zentrale Berechtigungsprüfung berücksichtigt Art, Beginn, Ende und wirksamen Status.
- [ ] **AK-02:** Kurse und Shop nutzen dieselbe fachliche Mitgliedschaftsquelle.
- [ ] **AK-03:** Noch ungeprüfter Antrag gilt nicht als aktive Mitgliedschaft.
- [ ] **AK-04:** Abgelaufene Mitgliedschaft erhält beim neuen Kauf keine Vorteile.
- [ ] **AK-05:** Preis-Snapshots bereits getätigter Käufe bleiben unverändert.
- [ ] **AK-06:** Manuelle Sonderregel benötigt Gültigkeit, Grund und berechtigte Freigabe.

## Abhängigkeiten und Voraussetzungen

[MIT-02 #63](https://github.com/marcbey/the-step-agentic-workflow/issues/63), [MIT-04 #69](https://github.com/marcbey/the-step-agentic-workflow/issues/69), [BUC-03 #49](https://github.com/marcbey/the-step-agentic-workflow/issues/49)

**Vor Umsetzung zu klären:** D12. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

User bezeichnet Zugang; Membership den Mitgliedschaftsstatus; Kind/Teilnehmer erhält nicht automatisch ein Login.

**Voraussichtliche Codeorte:** `app/models/membership.rb, app/models/guardian_relationship.rb, app/controllers/portal/, app/services/memberships/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Übergang exakt am Mitgliedschaftsende, offener Antrag und parallele Preisabfrage bei Kündigung prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
