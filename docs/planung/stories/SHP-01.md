# SHP-01 – Handelsmodell und Shopschnittstelle entscheiden

[GitHub-Issue #80](https://github.com/marcbey/the-step-agentic-workflow/issues/80)

## User Story

Als **Vereinsvorstand** möchte ich **Handelsmodell und Shopschnittstelle entscheiden**.

**Erwarteter Nutzen:** einen wirtschaftlich und organisatorisch tragbaren Shop aufzusetzen.

## Einordnung

- Story-ID: [SHP-01 #80](https://github.com/marcbey/the-step-agentic-workflow/issues/80) · Epic: [E10 #10](https://github.com/marcbey/the-step-agentic-workflow/issues/10)
- Release: **R3** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: F01, F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Verglichen werden integrierter Rails-Shop und angebundener gehosteter Shop.
- [ ] **AK-02:** Händler, Sortiment, Zahlungsanbieter, Versandgebiet und Verantwortliche sind benannt.
- [ ] **AK-03:** Mitgliederpreisprüfung und Bestell-/Rechnungsdatenflüsse sind beschrieben.
- [ ] **AK-04:** Betriebsaufwand, laufende Gebühren und Datenexport werden bewertet.
- [ ] **AK-05:** Katalog, Checkout, Bestellungen und Gutscheine haben unabhängig vom Anbieter klare Zuständigkeiten.
- [ ] **AK-06:** Entscheidung ist vor produktiver Checkout-Implementierung dokumentiert.

## Abhängigkeiten und Voraussetzungen

[MIT-05 #70](https://github.com/marcbey/the-step-agentic-workflow/issues/70), [FIN-01 #60](https://github.com/marcbey/the-step-agentic-workflow/issues/60), [GOV-02 #59](https://github.com/marcbey/the-step-agentic-workflow/issues/59)

**Vor Umsetzung zu klären:** D23. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Handelsanbieter wird hinter einer expliziten Grenze angebunden; Bestellung ist keine Kursbuchung.

**Voraussichtliche Codeorte:** `app/models/order.rb, app/models/voucher.rb, app/services/commerce/, app/controllers/shop/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Entscheidung anhand einer Beispielbestellung mit Mitgliederpreis, Retoure und Anbieter-Ausfall durchgehen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
