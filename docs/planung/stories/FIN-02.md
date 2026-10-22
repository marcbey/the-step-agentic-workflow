# FIN-02 – Zahlungen vor Ort und Forderungsstatus nachvollziehbar führen

[GitHub-Issue #61](https://github.com/marcbey/the-step-agentic-workflow/issues/61)

## User Story

Als **Kassenführung** möchte ich **Zahlungen vor Ort und Forderungsstatus nachvollziehbar führen**.

**Erwarteter Nutzen:** offene Beträge ohne vermeintliche Online-Zahlung zu erkennen.

## Einordnung

- Story-ID: [FIN-02 #61](https://github.com/marcbey/the-step-agentic-workflow/issues/61) · Epic: [E07 #7](https://github.com/marcbey/the-step-agentic-workflow/issues/7)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: T01, F04, F05; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** R1 übernimmt den vorhandenen internen Status offen/bezahlt als Zahlung-vor-Ort-Vermerk.
- [ ] **AK-02:** Status ist von Buchungsbestätigung und Teilnahme unabhängig.
- [ ] **AK-03:** Änderungen erfolgen nur durch fachlich berechtigte Personen mit Audit.
- [ ] **AK-04:** Gebührenfreie Buchungen erhalten keinen offenen Zahlungsstatus.
- [ ] **AK-05:** R2 definiert Teilzahlung, Rückzahlung und Korrektur als separate nachvollziehbare Buchungen.
- [ ] **AK-06:** Keine Zahlungsanbieter- oder Kartendaten werden im Kursformular gespeichert.

## Abhängigkeiten und Voraussetzungen

[BUC-03 #49](https://github.com/marcbey/the-step-agentic-workflow/issues/49), [BAS-03 #16](https://github.com/marcbey/the-step-agentic-workflow/issues/16)

**Vor Umsetzung zu klären:** D16. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Rechnung, Forderung, Zahlung und Buchungsstatus sind getrennte fachliche Größen; ganze Centwerte.

**Voraussichtliche Codeorte:** `app/models/invoice.rb, app/models/payment_entry.rb, app/services/billing/, app/controllers/admin/billing/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Nullbetrag, unberechtigter Coach, wiederholter Statuswechsel und anonymisierter Datensatz prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
