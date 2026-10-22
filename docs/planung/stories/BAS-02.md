# BAS-02 – Rails-Anwendung und reproduzierbare CI vorbereiten

[GitHub-Issue #15](https://github.com/marcbey/the-step-agentic-workflow/issues/15)

## User Story

Als **Entwicklung** möchte ich **Rails-Anwendung und reproduzierbare CI vorbereiten**.

**Erwarteter Nutzen:** einen reproduzierbaren Entwicklungs- und Prüfablauf.

## Einordnung

- Story-ID: [BAS-02 #15](https://github.com/marcbey/the-step-agentic-workflow/issues/15) · Epic: [E01 #1](https://github.com/marcbey/the-step-agentic-workflow/issues/1)
- Release: **R0** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: T01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Ruby 4.0.6 ist in mise und .ruby-version identisch festgelegt.
- [ ] **AK-02:** Rails 8.1.3.1 und sqlite3 2.9.6 werden über ein geprüftes Lockfile reproduziert.
- [ ] **AK-03:** Frischer Checkout lässt sich mit mise und db:prepare ohne Produktivdaten starten.
- [ ] **AK-04:** CI führt Minitest, Systemtests, RuboCop, Brakeman und Bundler Audit aus.
- [ ] **AK-05:** Secrets-, Datenbank- und private-Schlüssel-Dateien werden vom Commit ausgeschlossen und geprüft.
- [ ] **AK-06:** Fehlgeschlagene Pflichtprüfungen blockieren die technische Releasefreigabe.

## Abhängigkeiten und Voraussetzungen

[BAS-01 #14](https://github.com/marcbey/the-step-agentic-workflow/issues/14)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Rails-Boot, User/Session, zentrale Design-Tokens und Layout-Partials; kein zweites Identitätssystem.

**Voraussichtliche Codeorte:** `config/, Gemfile, .mise.toml, bin/ci, app/models/user.rb, app/assets/stylesheets/, app/views/layouts/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Frischen Checkout in CI vorbereiten; absichtlich fehlendes Secret und fehlerhaften Test als Negativfälle prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
