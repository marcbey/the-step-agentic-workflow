# KOM-01 – Kontaktanliegen und Gruppenanfragen zustellen

[GitHub-Issue #45](https://github.com/marcbey/the-step-agentic-workflow/issues/45)

## User Story

Als **Vereinsbüro** möchte ich **Kontaktanliegen und Gruppenanfragen zustellen**.

**Erwarteter Nutzen:** Anfragen dem richtigen Bearbeitungskanal zuzuordnen.

## Einordnung

- Story-ID: [KOM-01 #45](https://github.com/marcbey/the-step-agentic-workflow/issues/45) · Epic: [E06 #6](https://github.com/marcbey/the-step-agentic-workflow/issues/6)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: F04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Anliegen unterscheiden Kurs, Geburtstag, Mitgliedschaft, Kooperation und allgemeine Frage.
- [ ] **AK-02:** Bestätigung nennt eine Vorgangskennung ohne vertraulichen Inhalt.
- [ ] **AK-03:** Empfänger werden zentral konfiguriert und nicht aus Formularparametern übernommen.
- [ ] **AK-04:** Mailfehler behalten die Anfrage zur kontrollierten erneuten Zustellung.
- [ ] **AK-05:** Bearbeitungsstatus ist nur zuständigen Personen sichtbar.
- [ ] **AK-06:** Abgeschlossene Anfragen folgen einer freigegebenen Löschfrist.

## Abhängigkeiten und Voraussetzungen

[WEB-05 #36](https://github.com/marcbey/the-step-agentic-workflow/issues/36), [BAS-03 #16](https://github.com/marcbey/the-step-agentic-workflow/issues/16)

**Vor Umsetzung zu klären:** D04. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Eventanmeldung verwendet Booking; allgemeine Anfrage erzeugt ohne Prüfung keine Buchungsbestätigung.

**Voraussichtliche Codeorte:** `app/models/community_event.rb, app/models/contact_request.rb, app/mailers/, app/jobs/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Empfängermanipulation, doppelter Request und SMTP-Ausfall prüfen; Zugriff eines fremden Teams sperren.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
