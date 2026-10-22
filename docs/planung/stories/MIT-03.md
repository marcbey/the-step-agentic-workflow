# MIT-03 – Mitgliederdaten und Änderungen im Selbstservice pflegen

[GitHub-Issue #68](https://github.com/marcbey/the-step-agentic-workflow/issues/68)

## User Story

Als **Mitglied** möchte ich **Mitgliederdaten und Änderungen im Selbstservice pflegen**.

**Erwarteter Nutzen:** eigene Kontaktdaten aktuell zu halten.

## Einordnung

- Story-ID: [MIT-03 #68](https://github.com/marcbey/the-step-agentic-workflow/issues/68) · Epic: [E08 #8](https://github.com/marcbey/the-step-agentic-workflow/issues/8)
- Release: **R2** · Priorität: **P1** · vorläufige Größe: **5 Story Points**
- Quelle: F02, F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Mitglied sieht ausschließlich das eigene fachliche Profil.
- [ ] **AK-02:** Kontakt- und Adressänderungen werden validiert und nachvollziehbar gespeichert.
- [ ] **AK-03:** Neue E-Mail-Adresse wird vor Übernahme bestätigt.
- [ ] **AK-04:** Mitgliedsnummer, Beitragsart und Aufnahmestatus können nicht selbst manipuliert werden.
- [ ] **AK-05:** Bank-/Mandatsänderungen folgen gesondertem geschütztem Freigabeprozess.
- [ ] **AK-06:** Verwaltung erhält nur für notwendige Folgebearbeitung eine Änderungsmitteilung.

## Abhängigkeiten und Voraussetzungen

[MIT-02 #63](https://github.com/marcbey/the-step-agentic-workflow/issues/63), [MIT-06 #65](https://github.com/marcbey/the-step-agentic-workflow/issues/65)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

User bezeichnet Zugang; Membership den Mitgliedschaftsstatus; Kind/Teilnehmer erhält nicht automatisch ein Login.

**Voraussichtliche Codeorte:** `app/models/membership.rb, app/models/guardian_relationship.rb, app/controllers/portal/, app/services/memberships/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Fremde Mitglieds-ID, unbestätigte E-Mail und Manipulation des Beitragstyps über direkten Request prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
