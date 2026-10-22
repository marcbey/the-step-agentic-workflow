# EVT-02 – Online-Anmeldung für Veranstaltungen integrieren

[GitHub-Issue #57](https://github.com/marcbey/the-step-agentic-workflow/issues/57)

## User Story

Als **Eventbesucherin** möchte ich **Online-Anmeldung für Veranstaltungen integrieren**.

**Erwarteter Nutzen:** ohne separates System anmeldepflichtige Events zu buchen.

## Einordnung

- Story-ID: [EVT-02 #57](https://github.com/marcbey/the-step-agentic-workflow/issues/57) · Epic: [E06 #6](https://github.com/marcbey/the-step-agentic-workflow/issues/6)
- Release: **R1** · Priorität: **P1** · vorläufige Größe: **5 Story Points**
- Quelle: F03; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Event legt fest, ob Anmeldung notwendig, extern oder ohne Anmeldung möglich ist.
- [ ] **AK-02:** Interne Anmeldung verwendet Kapazitäts-, Minderjährigen- und Bestätigungsregeln der Buchung.
- [ ] **AK-03:** Kosten und Veranstalter sind vor Anmeldung sichtbar.
- [ ] **AK-04:** Eventabsage löst passende Benachrichtigung aus.
- [ ] **AK-05:** Externe Anmeldung wird vor Verlassen der Website deutlich bezeichnet.
- [ ] **AK-06:** Keine zusätzliche Kopie des Buchungsmodells wird eingeführt.

## Abhängigkeiten und Voraussetzungen

[EVT-01 #30](https://github.com/marcbey/the-step-agentic-workflow/issues/30), [BUC-02 #26](https://github.com/marcbey/the-step-agentic-workflow/issues/26), [BUC-04 #50](https://github.com/marcbey/the-step-agentic-workflow/issues/50)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Eventanmeldung verwendet Booking; allgemeine Anfrage erzeugt ohne Prüfung keine Buchungsbestätigung.

**Voraussichtliche Codeorte:** `app/models/community_event.rb, app/models/contact_request.rb, app/mailers/, app/jobs/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Kostenloses Event, volles Event und externes Ziel mit ungültiger URL prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
