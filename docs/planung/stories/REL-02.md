# REL-02 – Betriebsüberwachung und Störungsabläufe vorbereiten

[GitHub-Issue #93](https://github.com/marcbey/the-step-agentic-workflow/issues/93)

## User Story

Als **Betrieb** möchte ich **Betriebsüberwachung und Störungsabläufe vorbereiten**.

**Erwarteter Nutzen:** Ausfälle von Buchung, Mail und Hintergrundjobs rechtzeitig zu erkennen.

## Einordnung

- Story-ID: [REL-02 #93](https://github.com/marcbey/the-step-agentic-workflow/issues/93) · Epic: [E12 #12](https://github.com/marcbey/the-step-agentic-workflow/issues/12)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: T01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Healthchecks überwachen Web, Datenbanken, Queue und Scheduler getrennt.
- [ ] **AK-02:** Ausbleibende Reservierungsbereinigung und Mailrückstand erzeugen handlungsfähige Meldung.
- [ ] **AK-03:** SQLite-Schreibkonflikte, voller Datenträger und Backupfehler werden erkennbar.
- [ ] **AK-04:** Alarme enthalten keine Teilnehmerdaten und keine Tokens.
- [ ] **AK-05:** Runbook beschreibt Diagnose, sichere Wiederholung und Eskalationsverantwortung.
- [ ] **AK-06:** RPO höchstens 24 Stunden und RTO höchstens 4 Stunden gelten als zu bestätigende Planungsziele.

## Abhängigkeiten und Voraussetzungen

[BAS-04 #17](https://github.com/marcbey/the-step-agentic-workflow/issues/17), [BUC-04 #50](https://github.com/marcbey/the-step-agentic-workflow/issues/50), [GOV-03 #88](https://github.com/marcbey/the-step-agentic-workflow/issues/88)

**Vor Umsetzung zu klären:** D02. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Runbook und Handbuch folgen dem real implementierten Stand; Produktionsfreigabe ist keine Folge einer Issue-Anlage.

**Voraussichtliche Codeorte:** `docs/deployment.md, docs/runbooks/, app/views/admin/handbook/, .github/workflows/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Queue stoppen, Datenträgergrenze und fehlgeschlagenes Backup in Staging simulieren; alarmierten Wiederanlauf prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
