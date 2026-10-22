# WEB-02 – Verein, Geschichte und Abgrenzung zum Stuttpark darstellen

[GitHub-Issue #32](https://github.com/marcbey/the-step-agentic-workflow/issues/32)

## User Story

Als **Elternteil** möchte ich **Verein, Geschichte und Abgrenzung zum Stuttpark darstellen**.

**Erwarteter Nutzen:** Auftrag und Verantwortlichkeiten des Vereins zu verstehen.

## Einordnung

- Story-ID: [WEB-02 #32](https://github.com/marcbey/the-step-agentic-workflow/issues/32) · Epic: [E02 #2](https://github.com/marcbey/the-step-agentic-workflow/issues/2)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **3 Story Points**
- Quelle: F01, F03, W02; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Vereinsauftrag, Geschichte, Mission und Werte übernehmen die freigegebenen Referenzinhalte.
- [ ] **AK-02:** TheStep erscheint als Marke des Stuttgarter Skateboard e.V..
- [ ] **AK-03:** Stuttpark wird als Sportstätte und Infrastrukturpartner klar abgegrenzt.
- [ ] **AK-04:** Kurse, Camps, AGs, Workshops, Geburtstage, Firmenevents und Wettkämpfe sind zu passenden Angeboten verlinkt.
- [ ] **AK-05:** Vorstand, Mitgliedschaft, Satzung und Kinderschutz haben erkennbare Einstiege.
- [ ] **AK-06:** Redaktionelle Änderungen besitzen Vorschau, verantwortliche Freigabe und Änderungsdatum.

## Abhängigkeiten und Voraussetzungen

[BAS-06 #19](https://github.com/marcbey/the-step-agentic-workflow/issues/19), [CMS-01 #20](https://github.com/marcbey/the-step-agentic-workflow/issues/20)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Nur freigegebene Inhalte aus WebPage/Content::Repository und öffentlich gefilterte Fachdaten.

**Voraussichtliche Codeorte:** `app/controllers/pages_controller.rb, app/views/pages/, app/views/shared/, config/content/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Inhaltsabgleich mit Referenzseite einschließlich Gegenüberstellung Verein/Hallenbetrieb durchführen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
