# WEB-04 – Kinderschutzseite und verlässliche Kontaktwege bereitstellen

[GitHub-Issue #35](https://github.com/marcbey/the-step-agentic-workflow/issues/35)

## User Story

Als **Kind oder Elternteil** möchte ich **Kinderschutzseite und verlässliche Kontaktwege bereitstellen**.

**Erwarteter Nutzen:** das Schutzkonzept und freigegebene Hilfewege leicht zu finden.

## Einordnung

- Story-ID: [WEB-04 #35](https://github.com/marcbey/the-step-agentic-workflow/issues/35) · Epic: [E02 #2](https://github.com/marcbey/the-step-agentic-workflow/issues/2)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: F01, F02, W03, T01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Vollständiges Konzept wird als strukturierter HTML-Inhalt und zugänglicher Download angeboten.
- [ ] **AK-02:** Interne und externe Kinderschutzkontakte werden vom Verein fachlich bestätigt.
- [ ] **AK-03:** Fehlende oder ungeprüfte Kontakte blockieren das öffentliche Release.
- [ ] **AK-04:** Konzeptversion, Zuständigkeit und nächster Prüftermin sind nachvollziehbar.
- [ ] **AK-05:** Allgemeines Kontaktformular und öffentliche Kommentare werden nicht als vertrauliches Fallmanagement ausgegeben.
- [ ] **AK-06:** Kinderschutz ist von Angebotsdetail und Footer direkt erreichbar.

## Abhängigkeiten und Voraussetzungen

[CMS-01 #20](https://github.com/marcbey/the-step-agentic-workflow/issues/20), [WEB-07 #34](https://github.com/marcbey/the-step-agentic-workflow/issues/34)

**Vor Umsetzung zu klären:** D03. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Nur freigegebene Inhalte aus WebPage/Content::Repository und öffentlich gefilterte Fachdaten.

**Voraussichtliche Codeorte:** `app/controllers/pages_controller.rb, app/views/pages/, app/views/shared/, config/content/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Strikter Inhaltscheck muss bei fehlendem Kinderschutzkontakt scheitern und bei vollständig freigegebenen Angaben bestehen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
