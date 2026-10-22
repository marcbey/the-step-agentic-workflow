# BAS-04 – Isoliertes Staging und wiederherstellbares Deployment planen

[GitHub-Issue #17](https://github.com/marcbey/the-step-agentic-workflow/issues/17)

## User Story

Als **Betrieb** möchte ich **Isoliertes Staging und wiederherstellbares Deployment planen**.

**Erwarteter Nutzen:** neue Releases ohne Eingriff in das bestehende System prüfen zu können.

## Einordnung

- Story-ID: [BAS-04 #17](https://github.com/marcbey/the-step-agentic-workflow/issues/17) · Epic: [E01 #1](https://github.com/marcbey/the-step-agentic-workflow/issues/1)
- Release: **R0** · Priorität: **P0** · vorläufige Größe: **8 Story Points**
- Quelle: T01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Docker, GHCR, Kamal 2.12 und Hetzner folgen den Referenzkonventionen.
- [ ] **AK-02:** Neue Anwendung nutzt eigene Domain, Service-, Volume- und Datenbanknamen.
- [ ] **AK-03:** Webprozess, Solid Queue, Scheduler und Solid Cache starten mit Healthchecks.
- [ ] **AK-04:** SQLite- und Active-Storage-Daten bleiben über Deployments persistent.
- [ ] **AK-05:** Verschlüsselte konsistente Backups und Rückkehr auf den letzten freigegebenen Stand sind beschrieben.
- [ ] **AK-06:** Ein Restore in isoliertem Staging ist mit gesperrtem Mailversand erfolgreich nachgewiesen.

## Abhängigkeiten und Voraussetzungen

[BAS-02 #15](https://github.com/marcbey/the-step-agentic-workflow/issues/15)

**Vor Umsetzung zu klären:** D02. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Rails-Boot, User/Session, zentrale Design-Tokens und Layout-Partials; kein zweites Identitätssystem.

**Voraussichtliche Codeorte:** `config/, Gemfile, .mise.toml, bin/ci, app/models/user.rb, app/assets/stylesheets/, app/views/layouts/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Container ersetzen, Dateien und Datensätze wiederfinden; Restore und Rollback mit synthetischen Daten durchführen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
