# WEB-01 – Startseite mit aktuellen Einstiegen gestalten

[GitHub-Issue #31](https://github.com/marcbey/the-step-agentic-workflow/issues/31)

## User Story

Als **Interessentin** möchte ich **Startseite mit aktuellen Einstiegen gestalten**.

**Erwarteter Nutzen:** passende Angebote und Vereinsinformationen unmittelbar zu finden.

## Einordnung

- Story-ID: [WEB-01 #31](https://github.com/marcbey/the-step-agentic-workflow/issues/31) · Epic: [E02 #2](https://github.com/marcbey/the-step-agentic-workflow/issues/2)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: F01, F03, F05, W01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Hero übernimmt die Livegestaltung mit lesbarer Textalternative und statischem Fallback.
- [ ] **AK-02:** Primäre Aktion führt zu tatsächlich buchbaren Skateangeboten.
- [ ] **AK-03:** Nächste Trainings und Camps berücksichtigen Veröffentlichungsstatus und aktuelle Termine.
- [ ] **AK-04:** News und Events verwenden ausschließlich freigegebene Inhalte.
- [ ] **AK-05:** Vereinskurzvorstellung und Mitgliedschaftseinstieg sind erreichbar.
- [ ] **AK-06:** Test Seite, Foo, Beispielereignisse und redaktionelle Platzhalter werden nicht veröffentlicht.

## Abhängigkeiten und Voraussetzungen

[BAS-06 #19](https://github.com/marcbey/the-step-agentic-workflow/issues/19), [ANG-03 #27](https://github.com/marcbey/the-step-agentic-workflow/issues/27), [CMS-02 #29](https://github.com/marcbey/the-step-agentic-workflow/issues/29), [EVT-01 #30](https://github.com/marcbey/the-step-agentic-workflow/issues/30)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Nur freigegebene Inhalte aus WebPage/Content::Repository und öffentlich gefilterte Fachdaten.

**Voraussichtliche Codeorte:** `app/controllers/pages_controller.rb, app/views/pages/, app/views/shared/, config/content/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Leere Daten, vergangene Termine und deaktiviertes Video ergeben verständliche Ansichten ohne Musterinhalte.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
