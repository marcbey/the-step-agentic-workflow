# FIN-03 – Beitragsläufe und Finanzexporte vorbereiten

[GitHub-Issue #64](https://github.com/marcbey/the-step-agentic-workflow/issues/64)

## User Story

Als **Kassenführung** möchte ich **Beitragsläufe und Finanzexporte vorbereiten**.

**Erwarteter Nutzen:** Vereinsbeiträge kontrolliert einzuziehen oder abzurechnen.

## Einordnung

- Story-ID: [FIN-03 #64](https://github.com/marcbey/the-step-agentic-workflow/issues/64) · Epic: [E07 #7](https://github.com/marcbey/the-step-agentic-workflow/issues/7)
- Release: **R2** · Priorität: **P0** · vorläufige Größe: **8 Story Points**
- Quelle: F02, F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Beitrag wird anhand gültiger Beitragsordnung und Mitgliedschaftsart berechnet.
- [ ] **AK-02:** Vorschau zeigt fällige Personen, Beträge, Ausnahmen und Gesamtsumme.
- [ ] **AK-03:** Freigabe erzeugt pro Periode und Mitglied höchstens eine Forderung.
- [ ] **AK-04:** SEPA wird nur mit freigegebenem Mandatsmodell und gültigem Nachweis aktiviert.
- [ ] **AK-05:** Export enthält ausschließlich notwendige Finanzdaten und verhindert Tabellenformeln.
- [ ] **AK-06:** Rückläufer und Fehler werden ohne automatisches Beenden der Mitgliedschaft bearbeitet.

## Abhängigkeiten und Voraussetzungen

[MIT-01 #62](https://github.com/marcbey/the-step-agentic-workflow/issues/62), [MIT-02 #63](https://github.com/marcbey/the-step-agentic-workflow/issues/63), [FIN-01 #60](https://github.com/marcbey/the-step-agentic-workflow/issues/60)

**Vor Umsetzung zu klären:** D17. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Rechnung, Forderung, Zahlung und Buchungsstatus sind getrennte fachliche Größen; ganze Centwerte.

**Voraussichtliche Codeorte:** `app/models/invoice.rb, app/models/payment_entry.rb, app/services/billing/, app/controllers/admin/billing/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Wiederholter Lauf, Eintritt während der Periode, gekündigtes Mitglied und ungültiges Mandat prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
