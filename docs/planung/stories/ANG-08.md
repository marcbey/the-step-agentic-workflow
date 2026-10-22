# ANG-08 – Regelmäßige Kurse und Kursblöcke buchbar machen

[GitHub-Issue #48](https://github.com/marcbey/the-step-agentic-workflow/issues/48)

## User Story

Als **Mitglied** möchte ich **Regelmäßige Kurse und Kursblöcke buchbar machen**.

**Erwarteter Nutzen:** auch wiederkehrende Angebote online anzumelden.

## Einordnung

- Story-ID: [ANG-08 #48](https://github.com/marcbey/the-step-agentic-workflow/issues/48) · Epic: [E04 #4](https://github.com/marcbey/the-step-agentic-workflow/issues/4)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **8 Story Points**
- Quelle: F01, F03, T01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Referenzlücke der nicht buchbaren regelmäßigen Kurse ist ausdrücklich geschlossen.
- [ ] **AK-02:** Ein freigegebenes Modell unterscheidet Blockbuchung und einzelne Termine.
- [ ] **AK-03:** Bei Blockbuchung werden alle benötigten Plätze atomar geprüft.
- [ ] **AK-04:** Ein voller Teiltermin verhindert Teilbestätigung ohne bewusste Alternative.
- [ ] **AK-05:** Ferien, Ersatztermine und spätere Serienänderungen sind für die Buchung sichtbar.
- [ ] **AK-06:** Storno- und Preisregel für angebrochene Blöcke ist vor der Aktivierung dokumentiert.

## Abhängigkeiten und Voraussetzungen

[ANG-02 #22](https://github.com/marcbey/the-step-agentic-workflow/issues/22), [BUC-01 #25](https://github.com/marcbey/the-step-agentic-workflow/issues/25), [BUC-02 #26](https://github.com/marcbey/the-step-agentic-workflow/issues/26)

**Vor Umsetzung zu klären:** D10. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Angebot und einzelne Termine sind getrennt; Serien erzeugen keine zweite öffentliche Kapazitätsquelle.

**Voraussichtliche Codeorte:** `app/models/course_offering.rb, app/models/course_occurrence.rb, app/services/course_series_plan.rb, app/views/courses/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Block mit einem vollen Termin, verschobener Folgewoche und paralleler Block-/Einzelbuchung prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
