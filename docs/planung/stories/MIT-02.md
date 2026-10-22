# MIT-02 – Online-Mitgliedsantrag und Aufnahme bearbeiten

[GitHub-Issue #63](https://github.com/marcbey/the-step-agentic-workflow/issues/63)

## User Story

Als **antragstellende Person** möchte ich **Online-Mitgliedsantrag und Aufnahme bearbeiten**.

**Erwarteter Nutzen:** eine Vereinsmitgliedschaft digital beantragen zu können.

## Einordnung

- Story-ID: [MIT-02 #63](https://github.com/marcbey/the-step-agentic-workflow/issues/63) · Epic: [E08 #8](https://github.com/marcbey/the-step-agentic-workflow/issues/8)
- Release: **R2** · Priorität: **P0** · vorläufige Größe: **8 Story Points**
- Quelle: F02, F03; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Antrag erfasst nur die für die gewählte Mitgliedschaft erforderlichen Daten.
- [ ] **AK-02:** Minderjährige benötigen den festgelegten Erziehungsberechtigten-Nachweis.
- [ ] **AK-03:** Abgabe bestätigt den Eingang und behauptet noch keine Aufnahme.
- [ ] **AK-04:** Verwaltung kann Antrag prüfen, Rückfrage stellen, annehmen oder ablehnen.
- [ ] **AK-05:** Aufnahme erzeugt eindeutige Mitgliedsnummer, Startdatum und Status.
- [ ] **AK-06:** Satzungs-, Beitrags- und Datenschutzversion werden mit der Antragserklärung dokumentiert.

## Abhängigkeiten und Voraussetzungen

[MIT-01 #62](https://github.com/marcbey/the-step-agentic-workflow/issues/62), [BAS-03 #16](https://github.com/marcbey/the-step-agentic-workflow/issues/16), [GOV-01 #24](https://github.com/marcbey/the-step-agentic-workflow/issues/24)

**Vor Umsetzung zu klären:** D17. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

User bezeichnet Zugang; Membership den Mitgliedschaftsstatus; Kind/Teilnehmer erhält nicht automatisch ein Login.

**Voraussichtliche Codeorte:** `app/models/membership.rb, app/models/guardian_relationship.rb, app/controllers/portal/, app/services/memberships/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Doppelantrag, fehlende elterliche Vertretung, Ablehnung und erneuter Annahmeklick prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
