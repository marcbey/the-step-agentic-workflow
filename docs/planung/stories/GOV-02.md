# GOV-02 – Rechtstexte und Anbieterangaben kontrolliert übernehmen

[GitHub-Issue #59](https://github.com/marcbey/the-step-agentic-workflow/issues/59)

## User Story

Als **Vorstand** möchte ich **Rechtstexte und Anbieterangaben kontrolliert übernehmen**.

**Erwarteter Nutzen:** mit inhaltlich geprüften und funktionsgerechten Angaben zu veröffentlichen.

## Einordnung

- Story-ID: [GOV-02 #59](https://github.com/marcbey/the-step-agentic-workflow/issues/59) · Epic: [E11 #11](https://github.com/marcbey/the-step-agentic-workflow/issues/11)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: F04, W02, W03, W04, W05; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Verein, Kontakt, Impressum und Datenschutz beginnen mit den dokumentierten Referenzinhalten.
- [ ] **AK-02:** Rechtstexte besitzen Stand, Verantwortungsrolle und fachliche Freigabe.
- [ ] **AK-03:** Neue Datenflüsse für Mitgliedschaft, Kontaktformular, Shop und Kommunikation ergänzen die Referenz.
- [ ] **AK-04:** Bestehende Texte werden nicht als bereits ausreichende Freigabe neuer Funktionen ausgegeben.
- [ ] **AK-05:** Fehlende Pflichtangaben oder Platzhalter blockieren den betroffenen Release.
- [ ] **AK-06:** Datenschutzeinstellungen und Erklärung stimmen mit realen Netzwerkrequests überein.

## Abhängigkeiten und Voraussetzungen

[CMS-01 #20](https://github.com/marcbey/the-step-agentic-workflow/issues/20), [GOV-01 #24](https://github.com/marcbey/the-step-agentic-workflow/issues/24)

**Vor Umsetzung zu klären:** D03 D16 D23. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Berechtigung pro Request und Datei; separate Retention pro Datenart; keine pauschale Löschung von Finanzbelegen.

**Voraussichtliche Codeorte:** `app/policies/, app/jobs/retention/, config/initializers/, test/security/, test/system/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Inhaltsprüfung mit fehlendem Anbieter, unbekanntem Zahlungsanbieter und veralteter Consentbeschreibung muss scheitern.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
