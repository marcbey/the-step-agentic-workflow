# EXT-08 – Wetterinformationen für Outdoor-Angebote anzeigen

[GitHub-Issue #103](https://github.com/marcbey/the-step-agentic-workflow/issues/103)

## User Story

Als **Teilnehmerin** möchte ich **Wetterinformationen für Outdoor-Angebote anzeigen**.

**Erwarteter Nutzen:** die Wetteraussichten am Trainingsort einschätzen zu können.

## Einordnung

- Story-ID: [EXT-08 #103](https://github.com/marcbey/the-step-agentic-workflow/issues/103) · Epic: [E13 #13](https://github.com/marcbey/the-step-agentic-workflow/issues/13)
- Release: **R4** · Priorität: **P2** · vorläufige Größe: **5 Story Points**
- Quelle: F02, F05; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Nur tatsächlich als Outdoor markierte Angebote erhalten Wetterinformationen.
- [ ] **AK-02:** Anbieter, Standortbezug, Aktualisierungszeit und Quelle sind sichtbar.
- [ ] **AK-03:** Veraltete oder fehlende Daten werden nicht als aktuelle Vorhersage ausgegeben.
- [ ] **AK-04:** API-Ausfall verhindert weder Angebotsansicht noch Buchung.
- [ ] **AK-05:** Wetteranzeige löst keine automatische Absage oder Umbuchung aus.
- [ ] **AK-06:** Verbindliche Entscheidung und Regenregelung bleiben direkt erreichbar.

## Abhängigkeiten und Voraussetzungen

[ANG-01 #21](https://github.com/marcbey/the-step-agentic-workflow/issues/21), [BUC-09 #55](https://github.com/marcbey/the-step-agentic-workflow/issues/55)

**Vor Umsetzung zu klären:** D31. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Optionale Integration hat einen klaren Anbieter-/Datenvertrag und lässt Kernabläufe bei Ausfall nutzbar.

**Voraussichtliche Codeorte:** `app/services/integrations/, app/controllers/, app/views/, test/contracts/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** API-Timeout, alter Cache und verwechselter Trainingsort prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
