# MIT-07 – Geschützte Vereinsdokumente im Portal bereitstellen

[GitHub-Issue #71](https://github.com/marcbey/the-step-agentic-workflow/issues/71)

## User Story

Als **Mitglied** möchte ich **Geschützte Vereinsdokumente im Portal bereitstellen**.

**Erwarteter Nutzen:** interne freigegebene Unterlagen sicher abzurufen.

## Einordnung

- Story-ID: [MIT-07 #71](https://github.com/marcbey/the-step-agentic-workflow/issues/71) · Epic: [E08 #8](https://github.com/marcbey/the-step-agentic-workflow/issues/8)
- Release: **R2** · Priorität: **P1** · vorläufige Größe: **3 Story Points**
- Quelle: F02, F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Dokumente haben öffentliche, Mitglieder- oder Mitarbeiterfreigabe.
- [ ] **AK-02:** Mitgliedsstatus wird auch beim direkten Dateiabruf geprüft.
- [ ] **AK-03:** Version, Datum und zugängliche Beschreibung sind sichtbar.
- [ ] **AK-04:** Downloadlinks sind kurzlebig und nicht dauerhaft öffentlich.
- [ ] **AK-05:** Entzug der Berechtigung sperrt bestehende Verweise.
- [ ] **AK-06:** Nicht freigegebene Dokumente sind weder in Suche noch Sitemap enthalten.

## Abhängigkeiten und Voraussetzungen

[MIT-06 #65](https://github.com/marcbey/the-step-agentic-workflow/issues/65), [WEB-07 #34](https://github.com/marcbey/the-step-agentic-workflow/issues/34)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

User bezeichnet Zugang; Membership den Mitgliedschaftsstatus; Kind/Teilnehmer erhält nicht automatisch ein Login.

**Voraussichtliche Codeorte:** `app/models/membership.rb, app/models/guardian_relationship.rb, app/controllers/portal/, app/services/memberships/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Direktlink nach Kündigung, fremde Dokument-ID und Browsercache auf gemeinsamem Gerät prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
