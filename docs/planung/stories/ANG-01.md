# ANG-01 – Angebotsarten und veröffentlichbare Angebotsdaten modellieren

[GitHub-Issue #21](https://github.com/marcbey/the-step-agentic-workflow/issues/21)

## User Story

Als **Kursplanung** möchte ich **Angebotsarten und veröffentlichbare Angebotsdaten modellieren**.

**Erwarteter Nutzen:** Kurse, Schnuppern, Camps und Workshops einheitlich zu beschreiben.

## Einordnung

- Story-ID: [ANG-01 #21](https://github.com/marcbey/the-step-agentic-workflow/issues/21) · Epic: [E04 #4](https://github.com/marcbey/the-step-agentic-workflow/issues/4)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **8 Story Points**
- Quelle: F01, F03, T01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Angebotstyp, Alter, Level, Ort, Preisgruppen und Buchungsregeln sind typisierte Daten.
- [ ] **AK-02:** Regelmäßiger Kurs, Einzelkurs und mehrtägiges Angebot sind unterscheidbar.
- [ ] **AK-03:** Entwurf, veröffentlicht, abgesagt und archiviert haben klare Wirkung.
- [ ] **AK-04:** Kapazität und Buchungsschluss werden serverseitig validiert.
- [ ] **AK-05:** Nicht buchbare Angebote zeigen einen erklärten Kontakt- oder Anmeldeweg.
- [ ] **AK-06:** Es werden keine unbelegten Preise, Altersgrenzen oder Kursbestände als Fakten angelegt.

## Abhängigkeiten und Voraussetzungen

[BAS-02 #15](https://github.com/marcbey/the-step-agentic-workflow/issues/15), [CMS-01 #20](https://github.com/marcbey/the-step-agentic-workflow/issues/20)

**Vor Umsetzung zu klären:** D07. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Angebot und einzelne Termine sind getrennt; Serien erzeugen keine zweite öffentliche Kapazitätsquelle.

**Voraussichtliche Codeorte:** `app/models/course_offering.rb, app/models/course_occurrence.rb, app/services/course_series_plan.rb, app/views/courses/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Unvollständiges Angebot kann nicht veröffentlicht werden; vergangener Termin und negative Kapazität werden abgewiesen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
