# ANG-07 – Leihmaterial und Ausrüstung im Angebot berücksichtigen

[GitHub-Issue #23](https://github.com/marcbey/the-step-agentic-workflow/issues/23)

## User Story

Als **buchende Person** möchte ich **Leihmaterial und Ausrüstung im Angebot berücksichtigen**.

**Erwarteter Nutzen:** Ausrüstung und Zusatzkosten vor der Anmeldung zu kennen.

## Einordnung

- Story-ID: [ANG-07 #23](https://github.com/marcbey/the-step-agentic-workflow/issues/23) · Epic: [E04 #4](https://github.com/marcbey/the-step-agentic-workflow/issues/4)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: F02, F03, T01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Board, Helm und Schutzausrüstung sind einzeln konfigurierbare Leihkategorien.
- [ ] **AK-02:** Vorgegebene Leihgebühr beträgt im übernommenen Referenzmodell 5 Euro je Kategorie und Buchungseinheit.
- [ ] **AK-03:** Kosten werden ausschließlich auf dem Server berechnet.
- [ ] **AK-04:** Ausrüstungsbedarf bleibt in Bestätigung und Teilnehmerliste konsistent.
- [ ] **AK-05:** Hinweise zu eigener Ausrüstung und Schutzregeln sind direkt erreichbar.
- [ ] **AK-06:** Übernahme von Verzichtserklärungen erfolgt erst nach aktueller fachlicher Sicherheitsfreigabe.

## Abhängigkeiten und Voraussetzungen

[ANG-01 #21](https://github.com/marcbey/the-step-agentic-workflow/issues/21)

**Vor Umsetzung zu klären:** D09. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Angebot und einzelne Termine sind getrennt; Serien erzeugen keine zweite öffentliche Kapazitätsquelle.

**Voraussichtliche Codeorte:** `app/models/course_offering.rb, app/models/course_occurrence.rb, app/services/course_series_plan.rb, app/views/courses/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Manipulierten Browserpreis, mehrere Camptage und widersprüchliche Leihantworten prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
