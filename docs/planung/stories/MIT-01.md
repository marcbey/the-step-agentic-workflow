# MIT-01 – Mitgliedschaft, Beiträge und Vorteile verständlich erklären

[GitHub-Issue #62](https://github.com/marcbey/the-step-agentic-workflow/issues/62)

## User Story

Als **Vereinsinteressentin** möchte ich **Mitgliedschaft, Beiträge und Vorteile verständlich erklären**.

**Erwarteter Nutzen:** vor einem Antrag die Bedingungen zu verstehen.

## Einordnung

- Story-ID: [MIT-01 #62](https://github.com/marcbey/the-step-agentic-workflow/issues/62) · Epic: [E08 #8](https://github.com/marcbey/the-step-agentic-workflow/issues/8)
- Release: **R2** · Priorität: **P0** · vorläufige Größe: **3 Story Points**
- Quelle: F01, F02, F03, F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Aktive, Familien- und Fördermitgliedschaft werden nur gemäß beschlossener Ordnung angeboten.
- [ ] **AK-02:** Beitrag, Zahlungsrhythmus, Aufnahmebedingungen und Kündigungsregel sind sichtbar.
- [ ] **AK-03:** Vorteile unterscheiden Kursrabatt, Shoprabatt und sonstige Vereinsleistungen.
- [ ] **AK-04:** Aktuelle Satzung und Beitragsordnung sind direkt verlinkt.
- [ ] **AK-05:** Änderungen haben Version und Wirksamkeitsdatum.
- [ ] **AK-06:** Keine redaktionelle Vorteilsbeschreibung verspricht technisch noch nicht verfügbare Rabatte.

## Abhängigkeiten und Voraussetzungen

[WEB-02 #32](https://github.com/marcbey/the-step-agentic-workflow/issues/32), [WEB-07 #34](https://github.com/marcbey/the-step-agentic-workflow/issues/34)

**Vor Umsetzung zu klären:** D17. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

User bezeichnet Zugang; Membership den Mitgliedschaftsstatus; Kind/Teilnehmer erhält nicht automatisch ein Login.

**Voraussichtliche Codeorte:** `app/models/membership.rb, app/models/guardian_relationship.rb, app/controllers/portal/, app/services/memberships/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Vergleich veröffentlichter Beiträge mit Antrags- und Berechnungsansicht; zukünftige Ordnung darf nicht vorzeitig wirken.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
