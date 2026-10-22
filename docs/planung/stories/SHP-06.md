# SHP-06 – Bestellungen, Versand, Abholung und Retouren bearbeiten

[GitHub-Issue #85](https://github.com/marcbey/the-step-agentic-workflow/issues/85)

## User Story

Als **Shopteam** möchte ich **Bestellungen, Versand, Abholung und Retouren bearbeiten**.

**Erwarteter Nutzen:** Bestellungen nachvollziehbar bis zum Abschluss zu führen.

## Einordnung

- Story-ID: [SHP-06 #85](https://github.com/marcbey/the-step-agentic-workflow/issues/85) · Epic: [E10 #10](https://github.com/marcbey/the-step-agentic-workflow/issues/10)
- Release: **R3** · Priorität: **P0** · vorläufige Größe: **8 Story Points**
- Quelle: F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Bestellansicht unterscheidet Zahlung, Erfüllung, Versand und Retoure.
- [ ] **AK-02:** Nur fachlich freigegebene Liefer- und Abholarten sind wählbar.
- [ ] **AK-03:** Bestandskorrektur bei Rückgabe benötigt geprüftes Ergebnis.
- [ ] **AK-04:** Rückerstattung besitzt Referenz zur ursprünglichen Zahlung und Belegkorrektur.
- [ ] **AK-05:** Käufer erhält angemessene Bestell- und Versandinformationen.
- [ ] **AK-06:** Shopberechtigung gewährt keinen Zugriff auf Kinder- und Trainingsdaten.

## Abhängigkeiten und Voraussetzungen

[SHP-05 #84](https://github.com/marcbey/the-step-agentic-workflow/issues/84)

**Vor Umsetzung zu klären:** D23. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Handelsanbieter wird hinter einer expliziten Grenze angebunden; Bestellung ist keine Kursbuchung.

**Voraussichtliche Codeorte:** `app/models/order.rb, app/models/voucher.rb, app/services/commerce/, app/controllers/shop/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Teilretoure, verlorene Sendung, doppelte Erstattung und reine Shoprolle prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
