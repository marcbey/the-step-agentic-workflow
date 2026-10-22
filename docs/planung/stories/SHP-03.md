# SHP-03 – Mitgliederpreise sicher im Shop anwenden

[GitHub-Issue #82](https://github.com/marcbey/the-step-agentic-workflow/issues/82)

## User Story

Als **Mitglied** möchte ich **Mitgliederpreise sicher im Shop anwenden**.

**Erwarteter Nutzen:** freigegebene Shopvergünstigungen automatisch zu nutzen.

## Einordnung

- Story-ID: [SHP-03 #82](https://github.com/marcbey/the-step-agentic-workflow/issues/82) · Epic: [E10 #10](https://github.com/marcbey/the-step-agentic-workflow/issues/10)
- Release: **R3** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: F01, F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Preisermittlung fragt zentrale wirksame Mitgliedschaft ab.
- [ ] **AK-02:** Gast sieht Standardpreis und einen verständlichen Vorteils-Hinweis.
- [ ] **AK-03:** Rabattkombinationen und Ausschlüsse sind fachlich festgelegt.
- [ ] **AK-04:** Checkout prüft Berechtigung erneut vor verbindlichem Kauf.
- [ ] **AK-05:** Bestellung speichert Preis- und Berechtigungs-Snapshot.
- [ ] **AK-06:** Manipulierte Rabattparameter und abgelaufene Mitgliedschaft reduzieren den Preis nicht.

## Abhängigkeiten und Voraussetzungen

[SHP-02 #81](https://github.com/marcbey/the-step-agentic-workflow/issues/81), [MIT-05 #70](https://github.com/marcbey/the-step-agentic-workflow/issues/70)

**Vor Umsetzung zu klären:** D12. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Handelsanbieter wird hinter einer expliziten Grenze angebunden; Bestellung ist keine Kursbuchung.

**Voraussichtliche Codeorte:** `app/models/order.rb, app/models/voucher.rb, app/services/commerce/, app/controllers/shop/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Mitgliedschaft endet zwischen Warenkorb und Checkout; Rabatte werden im Browser manipuliert.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
