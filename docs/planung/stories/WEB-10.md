# WEB-10 – Öffentliche Suche und Suchmaschinenbasis anbieten

[GitHub-Issue #40](https://github.com/marcbey/the-step-agentic-workflow/issues/40)

## User Story

Als **Besucherin** möchte ich **Öffentliche Suche und Suchmaschinenbasis anbieten**.

**Erwarteter Nutzen:** veröffentlichte Angebote und Informationen zu finden.

## Einordnung

- Story-ID: [WEB-10 #40](https://github.com/marcbey/the-step-agentic-workflow/issues/40) · Epic: [E02 #2](https://github.com/marcbey/the-step-agentic-workflow/issues/2)
- Release: **R1** · Priorität: **P1** · vorläufige Größe: **5 Story Points**
- Quelle: F05; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Suche umfasst freigegebene Seiten, Angebote, News und Events.
- [ ] **AK-02:** Private Profile, Buchungen und interne Dokumente werden nie indexiert.
- [ ] **AK-03:** Treffer zeigen Titel, Bereich und verständlichen Ausschnitt.
- [ ] **AK-04:** Leere Suche, Tippfehler und keine Treffer haben hilfreiche Rückwege.
- [ ] **AK-05:** Sitemap, Canonical-Links, Metadaten und Redirects erhalten öffentliche Auffindbarkeit.
- [ ] **AK-06:** Staging, Vorschauen und persönliche Bereiche sind für Suchmaschinen gesperrt.

## Abhängigkeiten und Voraussetzungen

[CMS-01 #20](https://github.com/marcbey/the-step-agentic-workflow/issues/20), [ANG-03 #27](https://github.com/marcbey/the-step-agentic-workflow/issues/27), [EVT-01 #30](https://github.com/marcbey/the-step-agentic-workflow/issues/30)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Nur freigegebene Inhalte aus WebPage/Content::Repository und öffentlich gefilterte Fachdaten.

**Voraussichtliche Codeorte:** `app/controllers/pages_controller.rb, app/views/pages/, app/views/shared/, config/content/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Suchbegriff mit HTML, sehr langer Eingabe und internem Datensatz darf weder XSS noch Datenabfluss erzeugen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
