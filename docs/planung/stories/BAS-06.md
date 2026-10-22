# BAS-06 – Navigation und zugängliche Grundlayouts erstellen

[GitHub-Issue #19](https://github.com/marcbey/the-step-agentic-workflow/issues/19)

## User Story

Als **Besucherin** möchte ich **Navigation und zugängliche Grundlayouts erstellen**.

**Erwarteter Nutzen:** Angebote und Hilfen auf Mobilgerät und Desktop schnell zu erreichen.

## Einordnung

- Story-ID: [BAS-06 #19](https://github.com/marcbey/the-step-agentic-workflow/issues/19) · Epic: [E01 #1](https://github.com/marcbey/the-step-agentic-workflow/issues/1)
- Release: **R0** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: F05, F04, W01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Sieben Hauptbereiche Startseite, Skateangebote, Events, Verein, Shop, News und Mein TheStep sind vorgesehen.
- [ ] **AK-02:** Noch nicht freigegebene Bereiche erscheinen erst mit funktionsfähigem Ziel.
- [ ] **AK-03:** Kontakt, Kinderschutz, Impressum, Datenschutz und Einstellungen sind dauerhaft erreichbar.
- [ ] **AK-04:** Mobile Navigation ist per Tastatur bedienbar und gibt Fokus nach dem Schließen zurück.
- [ ] **AK-05:** 320 Pixel Breite und 200 Prozent Zoom erzeugen keinen horizontalen Inhaltsverlust.
- [ ] **AK-06:** Skip-Link, Landmarken und verständliche Seitentitel sind in allen Layouts vorhanden.

## Abhängigkeiten und Voraussetzungen

[BAS-05 #18](https://github.com/marcbey/the-step-agentic-workflow/issues/18)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Rails-Boot, User/Session, zentrale Design-Tokens und Layout-Partials; kein zweites Identitätssystem.

**Voraussichtliche Codeorte:** `config/, Gemfile, .mise.toml, bin/ci, app/models/user.rb, app/assets/stylesheets/, app/views/layouts/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Tastaturpfad von Navigation zur Buchung sowie Browser-Zoom und schmale Darstellung prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
