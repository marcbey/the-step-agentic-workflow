# GOV-05 – Berechtigungen, Verschlüsselung und Missbrauchsschutz prüfen

[GitHub-Issue #90](https://github.com/marcbey/the-step-agentic-workflow/issues/90)

## User Story

Als **Betrieb** möchte ich **Berechtigungen, Verschlüsselung und Missbrauchsschutz prüfen**.

**Erwarteter Nutzen:** persönliche Daten und kritische Aktionen zu schützen.

## Einordnung

- Story-ID: [GOV-05 #90](https://github.com/marcbey/the-step-agentic-workflow/issues/90) · Epic: [E11 #11](https://github.com/marcbey/the-step-agentic-workflow/issues/11)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **8 Story Points**
- Quelle: T01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Buchungs- und sensible Kontaktdaten verwenden freigegebene Active-Record-Verschlüsselung.
- [ ] **AK-02:** Fehlende produktive Schlüssel verhindern den Anwendungsstart.
- [ ] **AK-03:** CSRF-, Origin-, Session- und Rate-Limit-Prüfungen sichern schreibende Aktionen.
- [ ] **AK-04:** Tokenwerte und sensible Freitexte sind in Rails-, Proxy- und Fehlerlogs maskiert.
- [ ] **AK-05:** Rollen werden auf Listen-, Detail-, Schreib-, Datei- und Exportebene geprüft.
- [ ] **AK-06:** Abhängigkeitsscan und gezielte Negativtests sind vor jedem Release erfolgreich.

## Abhängigkeiten und Voraussetzungen

[BAS-03 #16](https://github.com/marcbey/the-step-agentic-workflow/issues/16), [BAS-04 #17](https://github.com/marcbey/the-step-agentic-workflow/issues/17), [BUC-02 #26](https://github.com/marcbey/the-step-agentic-workflow/issues/26)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Berechtigung pro Request und Datei; separate Retention pro Datenart; keine pauschale Löschung von Finanzbelegen.

**Voraussichtliche Codeorte:** `app/policies/, app/jobs/retention/, config/initializers/, test/security/, test/system/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** IDOR, CSRF, Login-Bruteforce, fehlender Cache, entzogene Rechte und Rohdownload außerhalb der Sitzung prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
