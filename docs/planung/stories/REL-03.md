# REL-03 – Benutzerhandbuch und rollenspezifische Schulung bereitstellen

[GitHub-Issue #94](https://github.com/marcbey/the-step-agentic-workflow/issues/94)

## User Story

Als **Verwaltung** möchte ich **Benutzerhandbuch und rollenspezifische Schulung bereitstellen**.

**Erwarteter Nutzen:** Buchungen und Vereinsbetrieb sicher bedienen zu können.

## Einordnung

- Story-ID: [REL-03 #94](https://github.com/marcbey/the-step-agentic-workflow/issues/94) · Epic: [E12 #12](https://github.com/marcbey/the-step-agentic-workflow/issues/12)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: T01, F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Handbuch deckt alle vorhandenen Verwaltungsrouten und Rollen ab.
- [ ] **AK-02:** Jede neue Funktion aktualisiert Bedienablauf, Rechte, Validierungen und Datenschutz im selben Änderungssatz.
- [ ] **AK-03:** Kursplanung, Check-in, Storno und Versandfehler haben konkrete Beispiele.
- [ ] **AK-04:** R2 ergänzt Mitgliedschaft, Beiträge und Mitarbeiterzeiten; R3 ergänzt Shop und Erstattungen.
- [ ] **AK-05:** Schulung verwendet ausschließlich synthetische Daten.
- [ ] **AK-06:** Mindestens eine Person je verantwortlicher Rolle führt Kernfälle erfolgreich ohne Entwicklerhilfe durch.

## Abhängigkeiten und Voraussetzungen

[BUC-08 #54](https://github.com/marcbey/the-step-agentic-workflow/issues/54), [BUC-09 #55](https://github.com/marcbey/the-step-agentic-workflow/issues/55)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Runbook und Handbuch folgen dem real implementierten Stand; Produktionsfreigabe ist keine Folge einer Issue-Anlage.

**Voraussichtliche Codeorte:** `docs/deployment.md, docs/runbooks/, app/views/admin/handbook/, .github/workflows/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Neue Verwaltungsperson führt Kursanlage, manuelle Buchung, Storno und Mailwiederholung anhand des Handbuchs durch.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
