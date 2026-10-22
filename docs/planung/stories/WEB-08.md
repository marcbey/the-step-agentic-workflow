# WEB-08 – Sponsoren und Kooperationen sichtbar machen

[GitHub-Issue #38](https://github.com/marcbey/the-step-agentic-workflow/issues/38)

## User Story

Als **potenzieller Sponsor** möchte ich **Sponsoren und Kooperationen sichtbar machen**.

**Erwarteter Nutzen:** bestehende Zusammenarbeit und Unterstützungsmöglichkeiten zu verstehen.

## Einordnung

- Story-ID: [WEB-08 #38](https://github.com/marcbey/the-step-agentic-workflow/issues/38) · Epic: [E02 #2](https://github.com/marcbey/the-step-agentic-workflow/issues/2)
- Release: **R1** · Priorität: **P1** · vorläufige Größe: **3 Story Points**
- Quelle: F01, F02; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Sponsoren und Kooperationspartner haben getrennte Kategorien.
- [ ] **AK-02:** Freigegebene Logos, Beschreibungen und Links sind redaktionell pflegbar.
- [ ] **AK-03:** Aktive Laufzeit steuert die öffentliche Sichtbarkeit.
- [ ] **AK-04:** Sponsor werden führt zu einem zuordenbaren Kontaktanliegen.
- [ ] **AK-05:** Externe Links sind klar benannt und öffnen keine unkontrollierten Skripte.
- [ ] **AK-06:** Logorechte und verantwortliche Freigabe sind vor Veröffentlichung dokumentiert.

## Abhängigkeiten und Voraussetzungen

[CMS-01 #20](https://github.com/marcbey/the-step-agentic-workflow/issues/20), [WEB-05 #36](https://github.com/marcbey/the-step-agentic-workflow/issues/36)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Nur freigegebene Inhalte aus WebPage/Content::Repository und öffentlich gefilterte Fachdaten.

**Voraussichtliche Codeorte:** `app/controllers/pages_controller.rb, app/views/pages/, app/views/shared/, config/content/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Abgelaufener Sponsor, fehlendes Logo und ungültige externe URL ergeben sichere Zustände.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
