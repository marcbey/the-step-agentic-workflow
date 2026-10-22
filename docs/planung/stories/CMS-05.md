# CMS-05 – Pressebereich und freigegebene Materialien bereitstellen

[GitHub-Issue #42](https://github.com/marcbey/the-step-agentic-workflow/issues/42)

## User Story

Als **Pressevertreterin** möchte ich **Pressebereich und freigegebene Materialien bereitstellen**.

**Erwarteter Nutzen:** verlässliche Vereinsinformationen und verwendbare Medien zu erhalten.

## Einordnung

- Story-ID: [CMS-05 #42](https://github.com/marcbey/the-step-agentic-workflow/issues/42) · Epic: [E03 #3](https://github.com/marcbey/the-step-agentic-workflow/issues/3)
- Release: **R1** · Priorität: **P1** · vorläufige Größe: **3 Story Points**
- Quelle: F02; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Pressekontakt und Vereinskurzporträt sind zentral erreichbar.
- [ ] **AK-02:** Presseberichte und Links werden mit Datum und Quelle gepflegt.
- [ ] **AK-03:** Pressefotos zeigen Credit und erlaubte Verwendungszwecke.
- [ ] **AK-04:** Downloadpakete enthalten ausschließlich freigegebene Dateien.
- [ ] **AK-05:** Entzug einer Freigabe entfernt betroffene Downloads.
- [ ] **AK-06:** Presseanfragen werden dem passenden Kontaktkanal zugeordnet.

## Abhängigkeiten und Voraussetzungen

[CMS-01 #20](https://github.com/marcbey/the-step-agentic-workflow/issues/20), [CMS-03 #28](https://github.com/marcbey/the-step-agentic-workflow/issues/28), [WEB-05 #36](https://github.com/marcbey/the-step-agentic-workflow/issues/36)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

WebPage und Community-Inhalte mit Action Text/Lexxy; Medien über Active Storage mit geprüften Sichtbarkeitsregeln.

**Voraussichtliche Codeorte:** `app/models/web_page.rb, app/models/community_*.rb, app/controllers/admin/, app/views/community/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Gesperrtes Bild darf nicht im Downloadpaket verbleiben; tote externe Presselinks werden redaktionell erkennbar.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
