# FIN-04 – Rechnungen und Buchungsbelege im eigenen Portal anzeigen

[GitHub-Issue #66](https://github.com/marcbey/the-step-agentic-workflow/issues/66)

## User Story

Als **Mitglied** möchte ich **Rechnungen und Buchungsbelege im eigenen Portal anzeigen**.

**Erwarteter Nutzen:** die eigenen Belege sicher wiederzufinden.

## Einordnung

- Story-ID: [FIN-04 #66](https://github.com/marcbey/the-step-agentic-workflow/issues/66) · Epic: [E07 #7](https://github.com/marcbey/the-step-agentic-workflow/issues/7)
- Release: **R2** · Priorität: **P1** · vorläufige Größe: **5 Story Points**
- Quelle: F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Portal listet nur Belege der eigenen freigegebenen Rechnungsempfängerbeziehung.
- [ ] **AK-02:** Belegzugriff prüft Berechtigung bei jedem Download.
- [ ] **AK-03:** Korrekturbelege sind mit Originalbelegen verknüpft.
- [ ] **AK-04:** Familienbeziehungen verleihen keine unbegrenzten Rechte auf fremde Belege.
- [ ] **AK-05:** Ausgestellte Belege bleiben nach Kontoschließung gemäß freigegebener Frist geschützt verfügbar.
- [ ] **AK-06:** Versandwiederholung ändert weder Rechnungsnummer noch Betrag.

## Abhängigkeiten und Voraussetzungen

[FIN-01 #60](https://github.com/marcbey/the-step-agentic-workflow/issues/60), [MIT-06 #65](https://github.com/marcbey/the-step-agentic-workflow/issues/65)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Rechnung, Forderung, Zahlung und Buchungsstatus sind getrennte fachliche Größen; ganze Centwerte.

**Voraussichtliche Codeorte:** `app/models/invoice.rb, app/models/payment_entry.rb, app/services/billing/, app/controllers/admin/billing/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Erratene Beleg-ID, entzogene Sorgeberechtigung, abgelaufener Link und Korrekturbeleg prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
