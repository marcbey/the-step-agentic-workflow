# CMS-04 – Videos und externe Medien mit Zustimmung anzeigen

[GitHub-Issue #41](https://github.com/marcbey/the-step-agentic-workflow/issues/41)

## User Story

Als **Besucherin** möchte ich **Videos und externe Medien mit Zustimmung anzeigen**.

**Erwarteter Nutzen:** Videos mit selbst gewählten Datenschutzeinstellungen anzusehen.

## Einordnung

- Story-ID: [CMS-04 #41](https://github.com/marcbey/the-step-agentic-workflow/issues/41) · Epic: [E03 #3](https://github.com/marcbey/the-step-agentic-workflow/issues/3)
- Release: **R1** · Priorität: **P1** · vorläufige Größe: **5 Story Points**
- Quelle: F02, W05, T01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Eigene MP4-/WebM-Dateien und validierte YouTube-/Vimeo-Links sind unterstützt.
- [ ] **AK-02:** Externe Anbieter erhalten vor aktiver Zustimmung keine Requests.
- [ ] **AK-03:** Ablehnung lässt Seite und Buchungswege vollständig nutzbar.
- [ ] **AK-04:** Zustimmung kann über Footer und Einbettungsplatzhalter geändert werden.
- [ ] **AK-05:** Widerruf entfernt externe Player und verhindert neue Anbieterrequests.
- [ ] **AK-06:** Bedeutungstragende Videos erhalten geplante Untertitel oder Textalternative vor inhaltlicher Freigabe.

## Abhängigkeiten und Voraussetzungen

[CMS-03 #28](https://github.com/marcbey/the-step-agentic-workflow/issues/28), [GOV-01 #24](https://github.com/marcbey/the-step-agentic-workflow/issues/24)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

WebPage und Community-Inhalte mit Action Text/Lexxy; Medien über Active Storage mit geprüften Sichtbarkeitsregeln.

**Voraussichtliche Codeorte:** `app/models/web_page.rb, app/models/community_*.rb, app/controllers/admin/, app/views/community/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Netzwerkrequests vor Zustimmung, nach Ablehnung und nach Widerruf prüfen; bösartige Embed-URLs ablehnen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
