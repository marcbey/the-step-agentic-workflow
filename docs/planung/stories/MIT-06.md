# MIT-06 – Mein TheStep und freigegebene Familienbeziehungen bereitstellen

[GitHub-Issue #65](https://github.com/marcbey/the-step-agentic-workflow/issues/65)

## User Story

Als **Erziehungsberechtigte** möchte ich **Mein TheStep und freigegebene Familienbeziehungen bereitstellen**.

**Erwarteter Nutzen:** eigene und berechtigt zugeordnete Kinderbuchungen zu verwalten.

## Einordnung

- Story-ID: [MIT-06 #65](https://github.com/marcbey/the-step-agentic-workflow/issues/65) · Epic: [E08 #8](https://github.com/marcbey/the-step-agentic-workflow/issues/8)
- Release: **R2** · Priorität: **P0** · vorläufige Größe: **8 Story Points**
- Quelle: F01, F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Ein Zugang zeigt eigene Buchungen, zugeordnete Kinder und Handlungsoptionen.
- [ ] **AK-02:** Beziehung zum Kind wird nach einem dokumentierten Nachweisverfahren freigegeben.
- [ ] **AK-03:** Gleiche E-Mail-Adresse oder gleicher Nachname genügt nicht zum Zusammenführen.
- [ ] **AK-04:** Zweiter Sorgeberechtigter erhält nur ausdrücklich freigegebenen Zugriff.
- [ ] **AK-05:** Widerruf oder Ende einer Beziehung sperrt den Zugriff beim nächsten Request.
- [ ] **AK-06:** Vorhandene Gastbuchungen werden ausschließlich über einen sicheren Anspruchsnachweis zugeordnet.

## Abhängigkeiten und Voraussetzungen

[BAS-03 #16](https://github.com/marcbey/the-step-agentic-workflow/issues/16), [MIT-02 #63](https://github.com/marcbey/the-step-agentic-workflow/issues/63), [BUC-02 #26](https://github.com/marcbey/the-step-agentic-workflow/issues/26)

**Vor Umsetzung zu klären:** D19. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

User bezeichnet Zugang; Membership den Mitgliedschaftsstatus; Kind/Teilnehmer erhält nicht automatisch ein Login.

**Voraussichtliche Codeorte:** `app/models/membership.rb, app/models/guardian_relationship.rb, app/controllers/portal/, app/services/memberships/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Namensgleichheit, geteilte E-Mail, entzogene Beziehung und beanspruchte fremde Gastbuchung prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
