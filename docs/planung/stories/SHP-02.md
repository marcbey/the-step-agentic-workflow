# SHP-02 – Produkte, Varianten und Vereinskollektion darstellen

[GitHub-Issue #81](https://github.com/marcbey/the-step-agentic-workflow/issues/81)

## User Story

Als **Käuferin** möchte ich **Produkte, Varianten und Vereinskollektion darstellen**.

**Erwarteter Nutzen:** passende Skateprodukte und Vereinsmerchandise auszuwählen.

## Einordnung

- Story-ID: [SHP-02 #81](https://github.com/marcbey/the-step-agentic-workflow/issues/81) · Epic: [E10 #10](https://github.com/marcbey/the-step-agentic-workflow/issues/10)
- Release: **R3** · Priorität: **P1** · vorläufige Größe: **5 Story Points**
- Quelle: F01, F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Kategorien decken Kleidung, Skateboards, Decks, Rollen, Zubehör und Vereinskollektion ab.
- [ ] **AK-02:** Varianten bilden Größe, Farbe und notwendige produktspezifische Merkmale ab.
- [ ] **AK-03:** Preise, Verfügbarkeit und freigegebene Produktbeschreibung sind sichtbar.
- [ ] **AK-04:** Produktbilder nutzen zentrale Rechte- und Alternativtextregeln.
- [ ] **AK-05:** Archivierte Produkte können nicht neu gekauft werden.
- [ ] **AK-06:** Leere Kategorien und ausverkaufte Varianten haben verständliche Zustände.

## Abhängigkeiten und Voraussetzungen

[SHP-01 #80](https://github.com/marcbey/the-step-agentic-workflow/issues/80), [CMS-03 #28](https://github.com/marcbey/the-step-agentic-workflow/issues/28)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Handelsanbieter wird hinter einer expliziten Grenze angebunden; Bestellung ist keine Kursbuchung.

**Voraussichtliche Codeorte:** `app/models/order.rb, app/models/voucher.rb, app/services/commerce/, app/controllers/shop/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Ausverkaufte Größe, fehlendes Bild und archivierte Variante über Direktlink prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
