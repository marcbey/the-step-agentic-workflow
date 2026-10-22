# BAS-05 – Bestehendes TheStep-Design als Komponentenbasis übernehmen

[GitHub-Issue #18](https://github.com/marcbey/the-step-agentic-workflow/issues/18)

## User Story

Als **Besucherin** möchte ich **Bestehendes TheStep-Design als Komponentenbasis übernehmen**.

**Erwarteter Nutzen:** TheStep im neuen Angebot wiederzuerkennen.

## Einordnung

- Story-ID: [BAS-05 #18](https://github.com/marcbey/the-step-agentic-workflow/issues/18) · Epic: [E01 #1](https://github.com/marcbey/the-step-agentic-workflow/issues/1)
- Release: **R0** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: W01, T01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Farbtokens #F5F0E6, #171717, #FFE500, #E5153D, #29B957 und #5421A6 sind zentral definiert.
- [ ] **AK-02:** Barlow Condensed, Bungee und Familjen Grotesk werden lokal mit Lizenznachweis ausgeliefert.
- [ ] **AK-03:** Schwarze Konturen, harte Schatten, gerade Karten und große Typografie entsprechen der Livevorlage.
- [ ] **AK-04:** Logo, Vereinsabsender und Hero mit SKATEBOARDING AGAINST LANGEWEILE sind anhand der aktuellen Website referenziert.
- [ ] **AK-05:** Buttons, Formulare, Fehlermeldungen, Statusanzeigen und Kalender besitzen gemeinsame Varianten.
- [ ] **AK-06:** Referenzansichten bei 375, 768 und 1440 Pixeln werden fachlich abgenommen.

## Abhängigkeiten und Voraussetzungen

[BAS-01 #14](https://github.com/marcbey/the-step-agentic-workflow/issues/14), [BAS-02 #15](https://github.com/marcbey/the-step-agentic-workflow/issues/15)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Rails-Boot, User/Session, zentrale Design-Tokens und Layout-Partials; kein zweites Identitätssystem.

**Voraussichtliche Codeorte:** `config/, Gemfile, .mise.toml, bin/ci, app/models/user.rb, app/assets/stylesheets/, app/views/layouts/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Komponentenansicht mit Fokus, Fehler, Ladezustand und langen deutschen Bezeichnungen visuell vergleichen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
