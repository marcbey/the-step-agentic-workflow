# EXT-03 – Bewertungen mit Moderation und Schutzregeln anbieten

[GitHub-Issue #98](https://github.com/marcbey/the-step-agentic-workflow/issues/98)

## User Story

Als **Teilnehmerin** möchte ich **Bewertungen mit Moderation und Schutzregeln anbieten**.

**Erwarteter Nutzen:** sachliches Feedback zu einem besuchten Angebot zu geben.

## Einordnung

- Story-ID: [EXT-03 #98](https://github.com/marcbey/the-step-agentic-workflow/issues/98) · Epic: [E13 #13](https://github.com/marcbey/the-step-agentic-workflow/issues/13)
- Release: **R4** · Priorität: **P2** · vorläufige Größe: **5 Story Points**
- Quelle: F05; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Bewertung ist auf nachgewiesene eigene Teilnahme begrenzt.
- [ ] **AK-02:** Öffentlichkeit und interne Rückmeldung sind ausdrücklich getrennt.
- [ ] **AK-03:** Veröffentlichung erfolgt moderiert ohne Kinder- oder Drittpersonendaten.
- [ ] **AK-04:** Melde- und Löschweg ist direkt erreichbar.
- [ ] **AK-05:** Mehrfache Bewertungen desselben Besuchs werden verhindert.
- [ ] **AK-06:** Absage, Löschung und Moderationsentscheidung bleiben nachvollziehbar.

## Abhängigkeiten und Voraussetzungen

[BUC-07 #53](https://github.com/marcbey/the-step-agentic-workflow/issues/53), [GOV-04 #89](https://github.com/marcbey/the-step-agentic-workflow/issues/89)

**Vor Umsetzung zu klären:** D29. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Optionale Integration hat einen klaren Anbieter-/Datenvertrag und lässt Kernabläufe bei Ausfall nutzbar.

**Voraussichtliche Codeorte:** `app/services/integrations/, app/controllers/, app/views/, test/contracts/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Nichtteilnehmer, personenbezogener Freitext und abgelehnte Veröffentlichung prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
