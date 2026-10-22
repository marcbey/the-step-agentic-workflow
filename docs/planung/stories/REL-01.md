# REL-01 – Inhalte und Bestandsdaten kontrolliert migrieren

[GitHub-Issue #92](https://github.com/marcbey/the-step-agentic-workflow/issues/92)

## User Story

Als **Projektverantwortung** möchte ich **Inhalte und Bestandsdaten kontrolliert migrieren**.

**Erwarteter Nutzen:** den Wechsel ohne Datenverlust und falsche Inhalte vorzubereiten.

## Einordnung

- Story-ID: [REL-01 #92](https://github.com/marcbey/the-step-agentic-workflow/issues/92) · Epic: [E12 #12](https://github.com/marcbey/the-step-agentic-workflow/issues/12)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **8 Story Points**
- Quelle: T01, W01, W02, W03, W04, W05; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Übernahmematrix unterscheidet öffentliche Texte, Medien, Konten und personenbezogene Fachbestände.
- [ ] **AK-02:** Nur freigegebene Inhalte und nachgewiesene Medienrechte werden übernommen.
- [ ] **AK-03:** Echter Datenimport hat eigenes Mapping, Trockenlauf und fachliche Stichprobe.
- [ ] **AK-04:** Historische Identitäts-Reset-Anweisungen werden nicht ungeprüft auf dieses neue Projekt angewandt.
- [ ] **AK-05:** Redirectliste und konsistentes Datenbank-/Storage-Backup sind Teil des Umschaltplans.
- [ ] **AK-06:** Rückfallkriterium, verantwortliche Person und Zeitraum der Schreibsperre sind vor Umschaltung festgelegt.

## Abhängigkeiten und Voraussetzungen

[BAS-01 #14](https://github.com/marcbey/the-step-agentic-workflow/issues/14), [BAS-04 #17](https://github.com/marcbey/the-step-agentic-workflow/issues/17), [GOV-02 #59](https://github.com/marcbey/the-step-agentic-workflow/issues/59), [GOV-03 #88](https://github.com/marcbey/the-step-agentic-workflow/issues/88)

**Vor Umsetzung zu klären:** D26. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Runbook und Handbuch folgen dem real implementierten Stand; Produktionsfreigabe ist keine Folge einer Issue-Anlage.

**Voraussichtliche Codeorte:** `docs/deployment.md, docs/runbooks/, app/views/admin/handbook/, .github/workflows/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Wiederholten Import, Sonderzeichen, fehlerhafte Verweise und Rückkehr auf Ausgangsstand proben.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
