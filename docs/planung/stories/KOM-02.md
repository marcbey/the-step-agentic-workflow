# KOM-02 – Newsletter mit bestätigter Anmeldung anbieten

[GitHub-Issue #58](https://github.com/marcbey/the-step-agentic-workflow/issues/58)

## User Story

Als **Interessentin** möchte ich **Newsletter mit bestätigter Anmeldung anbieten**.

**Erwarteter Nutzen:** freiwillig aktuelle Vereinsinformationen zu erhalten.

## Einordnung

- Story-ID: [KOM-02 #58](https://github.com/marcbey/the-step-agentic-workflow/issues/58) · Epic: [E06 #6](https://github.com/marcbey/the-step-agentic-workflow/issues/6)
- Release: **R2** · Priorität: **P1** · vorläufige Größe: **5 Story Points**
- Quelle: F05; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Newslettereinwilligung ist von Buchung und Mitgliedschaft getrennt.
- [ ] **AK-02:** Anmeldung wird erst nach Double-Opt-in aktiv.
- [ ] **AK-03:** Jede Ausgabe bietet einen wirksamen Abmeldelink ohne Login.
- [ ] **AK-04:** Einwilligungswortlaut, Zeitpunkt und Bestätigung sind nachweisbar.
- [ ] **AK-05:** Abgemeldete Kontakte werden vor jedem Versand ausgeschlossen.
- [ ] **AK-06:** Anbieter, Auftragsverarbeitung und Abmelde-/Löschprozess sind vor Aktivierung entschieden.

## Abhängigkeiten und Voraussetzungen

[GOV-01 #24](https://github.com/marcbey/the-step-agentic-workflow/issues/24)

**Vor Umsetzung zu klären:** D15. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Eventanmeldung verwendet Booking; allgemeine Anfrage erzeugt ohne Prüfung keine Buchungsbestätigung.

**Voraussichtliche Codeorte:** `app/models/community_event.rb, app/models/contact_request.rb, app/mailers/, app/jobs/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Unbestätigte Anmeldung, wiederholter Opt-in und Abmeldung nach Erstellen einer Versandliste prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
