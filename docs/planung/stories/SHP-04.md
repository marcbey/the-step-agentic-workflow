# SHP-04 – Warenkorb und bestandsfeste Reservierung umsetzen

[GitHub-Issue #83](https://github.com/marcbey/the-step-agentic-workflow/issues/83)

## User Story

Als **Käuferin** möchte ich **Warenkorb und bestandsfeste Reservierung umsetzen**.

**Erwarteter Nutzen:** nur verfügbare Ware zum angezeigten Preis zu bestellen.

## Einordnung

- Story-ID: [SHP-04 #83](https://github.com/marcbey/the-step-agentic-workflow/issues/83) · Epic: [E10 #10](https://github.com/marcbey/the-step-agentic-workflow/issues/10)
- Release: **R3** · Priorität: **P0** · vorläufige Größe: **8 Story Points**
- Quelle: F01, F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Warenkorb erfasst Variante und Menge mit serverseitiger Preisberechnung.
- [ ] **AK-02:** Mengen über Bestand und ungültige Varianten werden abgewiesen.
- [ ] **AK-03:** Begrenzte Checkoutreservierung wird mit Ablaufzeit geführt.
- [ ] **AK-04:** Parallele Käufe des letzten Artikels können den Bestand nicht negativ machen.
- [ ] **AK-05:** Ablauf oder Zahlungsabbruch gibt reservierten Bestand kontrolliert frei.
- [ ] **AK-06:** Mehrfacher Kaufklick mit gleichem Vorgang erzeugt keine Doppelbestellung.

## Abhängigkeiten und Voraussetzungen

[SHP-02 #81](https://github.com/marcbey/the-step-agentic-workflow/issues/81), [SHP-03 #82](https://github.com/marcbey/the-step-agentic-workflow/issues/82)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Handelsanbieter wird hinter einer expliziten Grenze angebunden; Bestellung ist keine Kursbuchung.

**Voraussichtliche Codeorte:** `app/models/order.rb, app/models/voucher.rb, app/services/commerce/, app/controllers/shop/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Zwei Checkoutprozesse für den letzten Artikel sowie Ablauf zeitgleich mit Zahlungsbestätigung prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
