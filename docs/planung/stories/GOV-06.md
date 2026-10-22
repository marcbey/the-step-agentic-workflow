# GOV-06 – Barrierefreiheit, Ladezeit und Browserqualität abnehmen

[GitHub-Issue #91](https://github.com/marcbey/the-step-agentic-workflow/issues/91)

## User Story

Als **Besucherin** möchte ich **Barrierefreiheit, Ladezeit und Browserqualität abnehmen**.

**Erwarteter Nutzen:** die Website mit unterschiedlichen Geräten und Hilfsmitteln zuverlässig zu nutzen.

## Einordnung

- Story-ID: [GOV-06 #91](https://github.com/marcbey/the-step-agentic-workflow/issues/91) · Epic: [E11 #11](https://github.com/marcbey/the-step-agentic-workflow/issues/11)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **8 Story Points**
- Quelle: F04, W01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** WCAG 2.2 AA ist als Qualitätsziel für Navigation, Inhalte und Formulare dokumentiert.
- [ ] **AK-02:** Kernabläufe sind vollständig mit Tastatur und verständlichen Fehlermeldungen nutzbar.
- [ ] **AK-03:** Videos respektieren reduzierte Bewegung und besitzen nutzbaren statischen Ersatz.
- [ ] **AK-04:** Repräsentative Seiten werden bei 375, 768 und 1440 Pixeln sowie 200 Prozent Zoom geprüft.
- [ ] **AK-05:** Für öffentliche Einstiege gelten Planungsbudgets LCP höchstens 2,5 Sekunden und CLS höchstens 0,1 unter dokumentiertem Messprofil.
- [ ] **AK-06:** Aktuelle Chromium-, Firefox- und WebKit-basierte Browser werden für kritische Abläufe geprüft.
- [ ] **AK-07:** Eine erreichbare Erklärung zur Barrierefreiheit beschreibt den tatsächlich geprüften Stand, bekannte Einschränkungen und einen Rückmeldeweg.

## Abhängigkeiten und Voraussetzungen

[BAS-06 #19](https://github.com/marcbey/the-step-agentic-workflow/issues/19), [WEB-01 #31](https://github.com/marcbey/the-step-agentic-workflow/issues/31), [BUC-02 #26](https://github.com/marcbey/the-step-agentic-workflow/issues/26), [CMS-04 #41](https://github.com/marcbey/the-step-agentic-workflow/issues/41)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Berechtigung pro Request und Datei; separate Retention pro Datenart; keine pauschale Löschung von Finanzbelegen.

**Voraussichtliche Codeorte:** `app/policies/, app/jobs/retention/, config/initializers/, test/security/, test/system/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Manuellen Screenreader-/Tastaturtest ergänzend zu automatischen Prüfungen und mobilem Kaltstart durchführen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
