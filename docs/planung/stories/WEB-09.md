# WEB-09 – Ehrenamt, Jobs, Praktikum und FSJ vorstellen

[GitHub-Issue #39](https://github.com/marcbey/the-step-agentic-workflow/issues/39)

## User Story

Als **Interessentin** möchte ich **Ehrenamt, Jobs, Praktikum und FSJ vorstellen**.

**Erwarteter Nutzen:** passende Möglichkeiten zur Mitarbeit zu finden.

## Einordnung

- Story-ID: [WEB-09 #39](https://github.com/marcbey/the-step-agentic-workflow/issues/39) · Epic: [E02 #2](https://github.com/marcbey/the-step-agentic-workflow/issues/2)
- Release: **R1** · Priorität: **P1** · vorläufige Größe: **3 Story Points**
- Quelle: F03; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Ehrenamt, Jobs, Praktikum und FSJ sind als getrennte Möglichkeiten beschreibbar.
- [ ] **AK-02:** Nur vom Verein bestätigte Stellen werden als offen bezeichnet.
- [ ] **AK-03:** Jedes Angebot zeigt Aufgaben, Voraussetzungen und Kontaktweg.
- [ ] **AK-04:** Abgelaufene Stellen verlieren ihre Bewerbungsaktion.
- [ ] **AK-05:** Bewerbungen werden an einen definierten geschützten Kanal verwiesen.
- [ ] **AK-06:** Für ein leeres Stellenangebot erscheint eine ehrliche Initiativkontakt-Option.

## Abhängigkeiten und Voraussetzungen

[CMS-01 #20](https://github.com/marcbey/the-step-agentic-workflow/issues/20), [WEB-05 #36](https://github.com/marcbey/the-step-agentic-workflow/issues/36)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Nur freigegebene Inhalte aus WebPage/Content::Repository und öffentlich gefilterte Fachdaten.

**Voraussichtliche Codeorte:** `app/controllers/pages_controller.rb, app/views/pages/, app/views/shared/, config/content/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Offene, geschlossene und fehlende Stellen samt direkter URL prüfen; keine Bewerbung im öffentlichen Newsbereich speichern.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
