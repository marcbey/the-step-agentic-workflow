# WEB-07 – Versionierte öffentliche Downloads bereitstellen

[GitHub-Issue #34](https://github.com/marcbey/the-step-agentic-workflow/issues/34)

## User Story

Als **Mitglied** möchte ich **Versionierte öffentliche Downloads bereitstellen**.

**Erwarteter Nutzen:** gültige Vereinsunterlagen einfach herunterzuladen.

## Einordnung

- Story-ID: [WEB-07 #34](https://github.com/marcbey/the-step-agentic-workflow/issues/34) · Epic: [E02 #2](https://github.com/marcbey/the-step-agentic-workflow/issues/2)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: F01, F02, F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Satzung, Beitragsordnung, Datenschutz, Einverständniserklärungen, Fördermitgliedsantrag und Flyer sind katalogisiert.
- [ ] **AK-02:** Jeder Download zeigt Titel, Dateityp, Größe, Version und Gültigkeit.
- [ ] **AK-03:** Nicht freigegebene und abgelaufene Fassungen erscheinen nicht als aktuell.
- [ ] **AK-04:** Dateityp und Dateigröße werden geprüft; Uploads enthalten keine unnötigen Unterschriften oder persönlichen Daten.
- [ ] **AK-05:** Wichtige PDF-Inhalte haben eine zugängliche HTML-Zusammenfassung.
- [ ] **AK-06:** Neue Versionen ersetzen den aktuellen Verweis ohne historische Belege ungültig zu machen.

## Abhängigkeiten und Voraussetzungen

[CMS-01 #20](https://github.com/marcbey/the-step-agentic-workflow/issues/20)

**Vor Umsetzung zu klären:** D05. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Nur freigegebene Inhalte aus WebPage/Content::Repository und öffentlich gefilterte Fachdaten.

**Voraussichtliche Codeorte:** `app/controllers/pages_controller.rb, app/views/pages/, app/views/shared/, config/content/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Berechtigung privater Dokumente, fehlerhafte PDF-Uploads, Versionswechsel und defekte Links prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
