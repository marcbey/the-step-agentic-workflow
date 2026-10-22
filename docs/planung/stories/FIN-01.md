# FIN-01 – Rechnungen und Korrekturbelege automatisch erstellen

[GitHub-Issue #60](https://github.com/marcbey/the-step-agentic-workflow/issues/60)

## User Story

Als **Kassenführung** möchte ich **Rechnungen und Korrekturbelege automatisch erstellen**.

**Erwarteter Nutzen:** bestätigte kostenpflichtige Leistungen nachvollziehbar abzurechnen.

## Einordnung

- Story-ID: [FIN-01 #60](https://github.com/marcbey/the-step-agentic-workflow/issues/60) · Epic: [E07 #7](https://github.com/marcbey/the-step-agentic-workflow/issues/7)
- Release: **R2** · Priorität: **P0** · vorläufige Größe: **8 Story Points**
- Quelle: F04, F05; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Beleg entsteht aus dem freigegebenen Leistungs- und Preis-Snapshot.
- [ ] **AK-02:** Nummern sind eindeutig und werden bei Parallelität nicht doppelt vergeben.
- [ ] **AK-03:** Ausgestellte Rechnungen sind unveränderlich; Korrektur erfolgt mit Referenzbeleg.
- [ ] **AK-04:** Steuer-, Pflichtangaben und gegebenenfalls E-Rechnungsformat sind vor Aktivierung geprüft.
- [ ] **AK-05:** PDF beziehungsweise freigegebenes strukturiertes Format und Versandstatus werden archiviert.
- [ ] **AK-06:** Kostenlose Leistungen erzeugen nur den festgelegten kostenfreien Nachweis.

## Abhängigkeiten und Voraussetzungen

[BUC-03 #49](https://github.com/marcbey/the-step-agentic-workflow/issues/49), [BUC-04 #50](https://github.com/marcbey/the-step-agentic-workflow/issues/50), [GOV-02 #59](https://github.com/marcbey/the-step-agentic-workflow/issues/59)

**Vor Umsetzung zu klären:** D16. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Rechnung, Forderung, Zahlung und Buchungsstatus sind getrennte fachliche Größen; ganze Centwerte.

**Voraussichtliche Codeorte:** `app/models/invoice.rb, app/models/payment_entry.rb, app/services/billing/, app/controllers/admin/billing/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Paralleler Rechnungslauf, nachträgliche Preisänderung, Storno nach Rechnung und erneuter Versand prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
