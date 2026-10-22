# BAS-03 – Konten, Rollen und Zuständigkeiten trennen

[GitHub-Issue #16](https://github.com/marcbey/the-step-agentic-workflow/issues/16)

## User Story

Als **Administration** möchte ich **Konten, Rollen und Zuständigkeiten trennen**.

**Erwarteter Nutzen:** Zugriffe passend zur jeweiligen Aufgabe vergeben zu können.

## Einordnung

- Story-ID: [BAS-03 #16](https://github.com/marcbey/the-step-agentic-workflow/issues/16) · Epic: [E01 #1](https://github.com/marcbey/the-step-agentic-workflow/issues/1)
- Release: **R0** · Priorität: **P0** · vorläufige Größe: **8 Story Points**
- Quelle: T01, F01, F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Ein User verwaltet Zugang und optionales öffentliches Teamprofil.
- [ ] **AK-02:** admin, editor und viewer bleiben Verwaltungsrollen; Coach ist eine zusätzliche Zuständigkeit.
- [ ] **AK-03:** Mitglied, Erziehungsberechtigte und Mitarbeitende erhalten getrennte fachliche Berechtigungen.
- [ ] **AK-04:** Anmeldung, Einladungsannahme, Passwortzurücksetzung und Logout haben ablaufende sichere Tokens.
- [ ] **AK-05:** Deaktivierung und Zuständigkeitsentzug wirken beim nächsten Request.
- [ ] **AK-06:** Der letzte aktive Admin kann weder gelöscht noch deaktiviert oder herabgestuft werden.

## Abhängigkeiten und Voraussetzungen

[BAS-02 #15](https://github.com/marcbey/the-step-agentic-workflow/issues/15)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Rails-Boot, User/Session, zentrale Design-Tokens und Layout-Partials; kein zweites Identitätssystem.

**Voraussichtliche Codeorte:** `config/, Gemfile, .mise.toml, bin/ci, app/models/user.rb, app/assets/stylesheets/, app/views/layouts/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Rollenmatrix einschließlich direkter URL-/ID-Manipulation und paralleler Änderungen am letzten Admin testen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
