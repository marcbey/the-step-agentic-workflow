# SHP-08 – Shopbedingungen und Rechnungskette freigeben

[GitHub-Issue #87](https://github.com/marcbey/the-step-agentic-workflow/issues/87)

## User Story

Als **Shopverantwortung** möchte ich **Shopbedingungen und Rechnungskette freigeben**.

**Erwarteter Nutzen:** den Handel mit aktuellen geprüften Informationen zu starten.

## Einordnung

- Story-ID: [SHP-08 #87](https://github.com/marcbey/the-step-agentic-workflow/issues/87) · Epic: [E10 #10](https://github.com/marcbey/the-step-agentic-workflow/issues/10)
- Release: **R3** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Impressum benennt den tatsächlich handelnden Anbieter.
- [ ] **AK-02:** Versand, Lieferzeiten, Rückgabe-/Widerrufsinformationen und Kaufbedingungen sind geprüft.
- [ ] **AK-03:** Preis-, Steuer- und Gutscheinangaben stimmen in Produkt, Checkout und Beleg überein.
- [ ] **AK-04:** Bestellbestätigung und Rechnung referenzieren denselben unveränderlichen Leistungsstand.
- [ ] **AK-05:** Datenschutz beschreibt tatsächlich eingesetzte Anbieter und Datenflüsse.
- [ ] **AK-06:** Ein dokumentierter Fachtest gibt Verkauf und Erstattungsprozess vor dem Start frei.

## Abhängigkeiten und Voraussetzungen

[SHP-01 #80](https://github.com/marcbey/the-step-agentic-workflow/issues/80), [SHP-05 #84](https://github.com/marcbey/the-step-agentic-workflow/issues/84), [SHP-06 #85](https://github.com/marcbey/the-step-agentic-workflow/issues/85), [SHP-07 #86](https://github.com/marcbey/the-step-agentic-workflow/issues/86), [GOV-02 #59](https://github.com/marcbey/the-step-agentic-workflow/issues/59)

**Vor Umsetzung zu klären:** D16 D23 D24. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Handelsanbieter wird hinter einer expliziten Grenze angebunden; Bestellung ist keine Kursbuchung.

**Voraussichtliche Codeorte:** `app/models/order.rb, app/models/voucher.rb, app/services/commerce/, app/controllers/shop/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Testkauf mit vollständiger Retoure und Gutscheinanteil bis zum Korrekturbeleg durchspielen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
