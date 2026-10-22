# WEB-06 – Service, Sicherheit und häufige Fragen pflegen

[GitHub-Issue #37](https://github.com/marcbey/the-step-agentic-workflow/issues/37)

## User Story

Als **Elternteil** möchte ich **Service, Sicherheit und häufige Fragen pflegen**.

**Erwarteter Nutzen:** Ausrüstung und Ablauf vor dem ersten Besuch zu kennen.

## Einordnung

- Story-ID: [WEB-06 #37](https://github.com/marcbey/the-step-agentic-workflow/issues/37) · Epic: [E02 #2](https://github.com/marcbey/the-step-agentic-workflow/issues/2)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **3 Story Points**
- Quelle: F02, F03; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** FAQ behandelt Alter, Level, Preise, Termine und Mitbringliste.
- [ ] **AK-02:** Wetter- und Regenregelung beschreibt Entscheidung, Kontaktweg und Ersatztermin.
- [ ] **AK-03:** Halleninformationen unterscheiden Vereinsangebot von Hallenöffnungszeiten und Eintritt.
- [ ] **AK-04:** Leihmaterial und Preise sind mit der aktuellen Angebotskonfiguration verknüpft.
- [ ] **AK-05:** Schutzausrüstung und Sicherheitshinweise sind auf relevanten Buchungswegen erreichbar.
- [ ] **AK-06:** FAQ kann ohne JavaScript gelesen und über direkte Abschnittslinks geteilt werden.

## Abhängigkeiten und Voraussetzungen

[ANG-01 #21](https://github.com/marcbey/the-step-agentic-workflow/issues/21), [CMS-01 #20](https://github.com/marcbey/the-step-agentic-workflow/issues/20)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Nur freigegebene Inhalte aus WebPage/Content::Repository und öffentlich gefilterte Fachdaten.

**Voraussichtliche Codeorte:** `app/controllers/pages_controller.rb, app/views/pages/, app/views/shared/, config/content/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Preisänderung darf keine abweichenden FAQ-Beträge erzeugen; Ankerlinks und No-JavaScript-Ansicht prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
