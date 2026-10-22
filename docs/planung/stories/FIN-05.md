# FIN-05 – Online-Zahlungsmodell für Angebote entscheiden

[GitHub-Issue #67](https://github.com/marcbey/the-step-agentic-workflow/issues/67)

## User Story

Als **Vereinsvorstand** möchte ich **Online-Zahlungsmodell für Angebote entscheiden**.

**Erwarteter Nutzen:** über Online-Zahlung anhand von Kosten und Betriebsfolgen zu entscheiden.

## Einordnung

- Story-ID: [FIN-05 #67](https://github.com/marcbey/the-step-agentic-workflow/issues/67) · Epic: [E07 #7](https://github.com/marcbey/the-step-agentic-workflow/issues/7)
- Release: **R3** · Priorität: **P1** · vorläufige Größe: **5 Story Points**
- Quelle: F05; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Entscheidung vergleicht Zahlung vor Ort, Überweisung und gehosteten Zahlungsanbieter.
- [ ] **AK-02:** Gebühren, Erstattungen, Buchhaltung, Datenflüsse und Verantwortliche sind dokumentiert.
- [ ] **AK-03:** Anbieter-Sandbox prüft Zahlung, Abbruch und Rückerstattung nur mit Testdaten.
- [ ] **AK-04:** Buchungsstatus, Forderung und Zahlungsstatus bleiben getrennt.
- [ ] **AK-05:** Doppelte und verspätete Webhooks sind Teil des freigegebenen Vertrags.
- [ ] **AK-06:** Aktivierung für Kurse erfolgt ausschließlich als eigener freigegebener Ausbau und ist kein R1-Blocker.

## Abhängigkeiten und Voraussetzungen

[FIN-01 #60](https://github.com/marcbey/the-step-agentic-workflow/issues/60), [FIN-02 #61](https://github.com/marcbey/the-step-agentic-workflow/issues/61)

**Vor Umsetzung zu klären:** D18. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Rechnung, Forderung, Zahlung und Buchungsstatus sind getrennte fachliche Größen; ganze Centwerte.

**Voraussichtliche Codeorte:** `app/models/invoice.rb, app/models/payment_entry.rb, app/services/billing/, app/controllers/admin/billing/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Entscheidungsnachweis und Sandboxprotokoll mit abgebrochener Zahlung und doppeltem Webhook vorlegen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
