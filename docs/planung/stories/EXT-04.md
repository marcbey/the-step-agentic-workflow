# EXT-04 – Englische Sprachversion für öffentliche Kernabläufe anbieten

[GitHub-Issue #99](https://github.com/marcbey/the-step-agentic-workflow/issues/99)

## User Story

Als **englischsprachige Person** möchte ich **Englische Sprachversion für öffentliche Kernabläufe anbieten**.

**Erwarteter Nutzen:** Angebote und Buchung zu verstehen.

## Einordnung

- Story-ID: [EXT-04 #99](https://github.com/marcbey/the-step-agentic-workflow/issues/99) · Epic: [E13 #13](https://github.com/marcbey/the-step-agentic-workflow/issues/13)
- Release: **R4** · Priorität: **P2** · vorläufige Größe: **8 Story Points**
- Quelle: F05; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Deutsch bleibt Ausgangssprache mit echten Umlauten.
- [ ] **AK-02:** Navigation, Angebotsdetails, Buchungsformular und Systemmails haben geprüfte englische Fassung.
- [ ] **AK-03:** Übersetzungen sind einem fachlichen Inhaltsstand zugeordnet.
- [ ] **AK-04:** Fehlende Übersetzung fällt sichtbar auf die freigegebene deutsche Fassung zurück.
- [ ] **AK-05:** Datums-, Zeit- und Währungsformate bleiben für den Standort eindeutig.
- [ ] **AK-06:** Sprachwechsel verliert weder ausgewähltes Angebot noch ungesendete Formulardaten.

## Abhängigkeiten und Voraussetzungen

[CMS-01 #20](https://github.com/marcbey/the-step-agentic-workflow/issues/20), [BUC-04 #50](https://github.com/marcbey/the-step-agentic-workflow/issues/50)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Optionale Integration hat einen klaren Anbieter-/Datenvertrag und lässt Kernabläufe bei Ausfall nutzbar.

**Voraussichtliche Codeorte:** `app/services/integrations/, app/controllers/, app/views/, test/contracts/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Unvollständig übersetztes Angebot, englische Fehlermeldung und Sprachwechsel im Formular prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
