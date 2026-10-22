# EXT-05 – WhatsApp als freiwilligen Kontaktweg verlinken

[GitHub-Issue #100](https://github.com/marcbey/the-step-agentic-workflow/issues/100)

## User Story

Als **Interessentin** möchte ich **WhatsApp als freiwilligen Kontaktweg verlinken**.

**Erwarteter Nutzen:** den Verein über einen bekannten optionalen Kanal zu erreichen.

## Einordnung

- Story-ID: [EXT-05 #100](https://github.com/marcbey/the-step-agentic-workflow/issues/100) · Epic: [E13 #13](https://github.com/marcbey/the-step-agentic-workflow/issues/13)
- Release: **R4** · Priorität: **P2** · vorläufige Größe: **3 Story Points**
- Quelle: F05; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Es wird ausschließlich eine bestätigte geschäftliche Kontaktadresse verwendet.
- [ ] **AK-02:** Ein einfacher externer Link löst vor dem Klick keine Anbieterrequests aus.
- [ ] **AK-03:** Hinweis benennt den externen Anbieter vor dem Wechsel.
- [ ] **AK-04:** Alternative per E-Mail und Telefon bleibt gleichwertig erreichbar.
- [ ] **AK-05:** Keine Teilnehmer- oder Kinderdaten werden automatisch in Linktexte übernommen.
- [ ] **AK-06:** Automatisierter Versand und Gruppenaufnahme sind nicht Teil dieser Story.

## Abhängigkeiten und Voraussetzungen

[WEB-05 #36](https://github.com/marcbey/the-step-agentic-workflow/issues/36), [GOV-02 #59](https://github.com/marcbey/the-step-agentic-workflow/issues/59)

**Vor Umsetzung zu klären:** D04. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Optionale Integration hat einen klaren Anbieter-/Datenvertrag und lässt Kernabläufe bei Ausfall nutzbar.

**Voraussichtliche Codeorte:** `app/services/integrations/, app/controllers/, app/views/, test/contracts/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Seitenaufruf ohne Klick und Link auf Mobil/Desktop prüfen; keine automatische Kontaktübermittlung.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
