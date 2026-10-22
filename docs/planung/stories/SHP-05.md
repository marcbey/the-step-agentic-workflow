# SHP-05 – Gehosteten Checkout und Zahlungsrückmeldungen integrieren

[GitHub-Issue #84](https://github.com/marcbey/the-step-agentic-workflow/issues/84)

## User Story

Als **Käuferin** möchte ich **Gehosteten Checkout und Zahlungsrückmeldungen integrieren**.

**Erwarteter Nutzen:** einen Kauf sicher abschließen zu können.

## Einordnung

- Story-ID: [SHP-05 #84](https://github.com/marcbey/the-step-agentic-workflow/issues/84) · Epic: [E10 #10](https://github.com/marcbey/the-step-agentic-workflow/issues/10)
- Release: **R3** · Priorität: **P0** · vorläufige Größe: **13 Story Points**
- Quelle: F01, F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Checkout zeigt Gesamtpreis, Versand, Steuerdarstellung und Händler vor Abschluss.
- [ ] **AK-02:** Kartendaten verbleiben beim freigegebenen Zahlungsanbieter.
- [ ] **AK-03:** Signierte Webhooks werden auf Herkunft, Ereignis-ID und Betrag geprüft.
- [ ] **AK-04:** Browserrückkehr allein markiert keine Bestellung als bezahlt.
- [ ] **AK-05:** Doppelte, verspätete und ungeordnete Ereignisse erzeugen keine doppelten Bestands- oder Belegaktionen.
- [ ] **AK-06:** Abbruch und Anbieter-Ausfall lassen einen verständlichen kontrollierten Wiederaufnahmeweg.

## Abhängigkeiten und Voraussetzungen

[SHP-04 #83](https://github.com/marcbey/the-step-agentic-workflow/issues/83), [FIN-01 #60](https://github.com/marcbey/the-step-agentic-workflow/issues/60)

**Vor Umsetzung zu klären:** D23. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Handelsanbieter wird hinter einer expliziten Grenze angebunden; Bestellung ist keine Kursbuchung.

**Voraussichtliche Codeorte:** `app/models/order.rb, app/models/voucher.rb, app/services/commerce/, app/controllers/shop/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Anbietersandbox: bezahlt ohne Browserrückkehr, falscher Betrag, doppelte Webhooks, verspätete Zahlung nach Reservierungsablauf.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
