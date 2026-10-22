# SHP-07 – Digitale Geschenkgutscheine ausgeben und einlösen

[GitHub-Issue #86](https://github.com/marcbey/the-step-agentic-workflow/issues/86)

## User Story

Als **schenkende Person** möchte ich **Digitale Geschenkgutscheine ausgeben und einlösen**.

**Erwarteter Nutzen:** einen Gutschein mit nachvollziehbarem Restwert zu verschenken.

## Einordnung

- Story-ID: [SHP-07 #86](https://github.com/marcbey/the-step-agentic-workflow/issues/86) · Epic: [E10 #10](https://github.com/marcbey/the-step-agentic-workflow/issues/10)
- Release: **R3** · Priorität: **P0** · vorläufige Größe: **8 Story Points**
- Quelle: F01, F04, F05; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Freigegebenes Modell unterscheidet Wertgutschein und zweckgebundenen Kursgutschein.
- [ ] **AK-02:** Code ist nicht erratbar und erscheint nicht in Logs.
- [ ] **AK-03:** Ausgabe erfolgt nach bestätigter Zahlung beziehungsweise berechtigter manueller Freigabe.
- [ ] **AK-04:** Einlösung und Restwertänderung sind atomar und historisch nachvollziehbar.
- [ ] **AK-05:** Storno und Erstattung berücksichtigen Gutscheinanteil und gegebenenfalls Restwert.
- [ ] **AK-06:** Gültigkeit, Übertragbarkeit und steuerliche Behandlung sind vor Verkauf festgelegt.

## Abhängigkeiten und Voraussetzungen

[SHP-05 #84](https://github.com/marcbey/the-step-agentic-workflow/issues/84), [FIN-01 #60](https://github.com/marcbey/the-step-agentic-workflow/issues/60)

**Vor Umsetzung zu klären:** D24. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Handelsanbieter wird hinter einer expliziten Grenze angebunden; Bestellung ist keine Kursbuchung.

**Voraussichtliche Codeorte:** `app/models/order.rb, app/models/voucher.rb, app/services/commerce/, app/controllers/shop/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Gleichzeitige Einlösung desselben Restwerts, Teilbetrag, ungültiger Code und Rückerstattung prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
