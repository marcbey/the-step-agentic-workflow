# ANG-06 – Schul-AGs, Gruppen und Firmenevents als Anfrage anbieten

[GitHub-Issue #47](https://github.com/marcbey/the-step-agentic-workflow/issues/47)

## User Story

Als **Kooperationspartner** möchte ich **Schul-AGs, Gruppen und Firmenevents als Anfrage anbieten**.

**Erwarteter Nutzen:** ein passendes betreutes Gruppenangebot zu erhalten.

## Einordnung

- Story-ID: [ANG-06 #47](https://github.com/marcbey/the-step-agentic-workflow/issues/47) · Epic: [E04 #4](https://github.com/marcbey/the-step-agentic-workflow/issues/4)
- Release: **R2** · Priorität: **P1** · vorläufige Größe: **5 Story Points**
- Quelle: F03, F05, W02; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Formular unterscheidet Schul-AG, Workshop, Firmenevent und sonstige Gruppe.
- [ ] **AK-02:** Gruppengröße, Zeitraum, Ort und organisatorische Kontaktperson sind erfassbar.
- [ ] **AK-03:** Es werden keine vollständigen Kinderlisten in der Erstanfrage verlangt.
- [ ] **AK-04:** Angebot und Zuordnung zur zuständigen Planung sind nachvollziehbar.
- [ ] **AK-05:** Bestätigung übernimmt geprüfte Termine und Kapazitäten in die Einsatzplanung.
- [ ] **AK-06:** Unverbindliche Anfrage ist optisch und in E-Mails von einer Buchung getrennt.

## Abhängigkeiten und Voraussetzungen

[ANG-01 #21](https://github.com/marcbey/the-step-agentic-workflow/issues/21), [WEB-05 #36](https://github.com/marcbey/the-step-agentic-workflow/issues/36), [KOM-01 #45](https://github.com/marcbey/the-step-agentic-workflow/issues/45)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Angebot und einzelne Termine sind getrennt; Serien erzeugen keine zweite öffentliche Kapazitätsquelle.

**Voraussichtliche Codeorte:** `app/models/course_offering.rb, app/models/course_occurrence.rb, app/services/course_series_plan.rb, app/views/courses/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Mehrere Alternativtermine, fehlende Kontaktadresse und falsche personenbezogene Uploads prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
