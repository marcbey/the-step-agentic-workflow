# OPS-04 – Stunden prüfen, freigeben und exportieren

[GitHub-Issue #76](https://github.com/marcbey/the-step-agentic-workflow/issues/76)

## User Story

Als **Koordination** möchte ich **Stunden prüfen, freigeben und exportieren**.

**Erwarteter Nutzen:** geprüfte Stunden an die Abrechnung zu übergeben.

## Einordnung

- Story-ID: [OPS-04 #76](https://github.com/marcbey/the-step-agentic-workflow/issues/76) · Epic: [E09 #9](https://github.com/marcbey/the-step-agentic-workflow/issues/9)
- Release: **R2** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Zuständige prüfende Person sieht eingereichte Einträge im freigegebenen Bereich.
- [ ] **AK-02:** Freigeben und Zurückweisen dokumentiert Bearbeiter, Zeitpunkt und Kommentar.
- [ ] **AK-03:** Eigene Freigabe wird nach dokumentierter Vier-Augen-Regel verhindert.
- [ ] **AK-04:** Freigegebene Zeit kann nur durch nachvollziehbare Korrektur geändert werden.
- [ ] **AK-05:** Periodenexport enthält nur geprüfte Stunden und schützt vor Tabellenformeln.
- [ ] **AK-06:** Export ist keine automatische Gehalts- oder Honorarzahlung.

## Abhängigkeiten und Voraussetzungen

[OPS-03 #75](https://github.com/marcbey/the-step-agentic-workflow/issues/75)

**Vor Umsetzung zu klären:** D21. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Operative Zugriffskontrolle verwendet aktive Zuordnung und Zeitfenster; Verwaltung und Coach bleiben getrennt.

**Voraussichtliche Codeorte:** `app/models/coach_assignment.rb, app/models/time_entry.rb, app/models/material_item.rb, app/controllers/staff/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Selbstfreigabe, nachträgliche Änderung und doppelte Periodenübergabe prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
