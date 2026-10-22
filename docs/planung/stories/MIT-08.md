# MIT-08 – Elternhilfe und Ehrenamtseinsätze organisieren

[GitHub-Issue #72](https://github.com/marcbey/the-step-agentic-workflow/issues/72)

## User Story

Als **Elternteil** möchte ich **Elternhilfe und Ehrenamtseinsätze organisieren**.

**Erwarteter Nutzen:** freiwillig bei passenden Vereinsaufgaben zu helfen.

## Einordnung

- Story-ID: [MIT-08 #72](https://github.com/marcbey/the-step-agentic-workflow/issues/72) · Epic: [E08 #8](https://github.com/marcbey/the-step-agentic-workflow/issues/8)
- Release: **R2** · Priorität: **P1** · vorläufige Größe: **5 Story Points**
- Quelle: F01, F03; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Verein veröffentlicht Aufgabe, Termin, Ort und benötigte Helferzahl.
- [ ] **AK-02:** Anmeldung zur Hilfe ist freiwillig und von Kursbuchung getrennt.
- [ ] **AK-03:** Eltern sehen eigene Zusagen und einen einfachen Rücktrittsweg.
- [ ] **AK-04:** Koordination sieht nur notwendige Kontaktdaten zugesagter Helfer.
- [ ] **AK-05:** Überbelegung eines Helferslots wird verhindert.
- [ ] **AK-06:** Absage und Änderung informieren ausschließlich betroffene Helfer.

## Abhängigkeiten und Voraussetzungen

[MIT-06 #65](https://github.com/marcbey/the-step-agentic-workflow/issues/65), [EVT-01 #30](https://github.com/marcbey/the-step-agentic-workflow/issues/30), [BUC-04 #50](https://github.com/marcbey/the-step-agentic-workflow/issues/50)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

User bezeichnet Zugang; Membership den Mitgliedschaftsstatus; Kind/Teilnehmer erhält nicht automatisch ein Login.

**Voraussichtliche Codeorte:** `app/models/membership.rb, app/models/guardian_relationship.rb, app/controllers/portal/, app/services/memberships/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Letzten Helferslot parallel belegen, Rücktritt und abgesagte Veranstaltung prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
