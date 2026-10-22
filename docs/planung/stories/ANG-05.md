# ANG-05 – Geburtstage vom Wunschtermin bis zur Bestätigung abwickeln

[GitHub-Issue #46](https://github.com/marcbey/the-step-agentic-workflow/issues/46)

## User Story

Als **Elternteil** möchte ich **Geburtstage vom Wunschtermin bis zur Bestätigung abwickeln**.

**Erwarteter Nutzen:** ein betreutes Geburtstagsangebot verbindlich vereinbaren zu können.

## Einordnung

- Story-ID: [ANG-05 #46](https://github.com/marcbey/the-step-agentic-workflow/issues/46) · Epic: [E04 #4](https://github.com/marcbey/the-step-agentic-workflow/issues/4)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **8 Story Points**
- Quelle: F01, F05; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Anfrage erfasst Wunschtermin, Gruppe, Alter und verantwortliche Kontaktperson.
- [ ] **AK-02:** Anfrage bestätigt ausschließlich den Eingang und blockiert noch keinen Kursplatz.
- [ ] **AK-03:** Planung prüft Ort, Betreuung und verfügbare Zeitfenster.
- [ ] **AK-04:** Ein befristetes Angebot nennt Leistungen, Kosten und Stornobedingungen.
- [ ] **AK-05:** Annahme und Freigabe durch Planung erzeugen eine verbindliche bestätigte Veranstaltung.
- [ ] **AK-06:** Ablehnung, Gegenangebot und Fristablauf sind dokumentiert und verständlich kommuniziert.

## Abhängigkeiten und Voraussetzungen

[ANG-01 #21](https://github.com/marcbey/the-step-agentic-workflow/issues/21), [WEB-05 #36](https://github.com/marcbey/the-step-agentic-workflow/issues/36), [KOM-01 #45](https://github.com/marcbey/the-step-agentic-workflow/issues/45)

**Vor Umsetzung zu klären:** D08. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Angebot und einzelne Termine sind getrennt; Serien erzeugen keine zweite öffentliche Kapazitätsquelle.

**Voraussichtliche Codeorte:** `app/models/course_offering.rb, app/models/course_occurrence.rb, app/services/course_series_plan.rb, app/views/courses/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Zwei Anfragen für dasselbe Zeitfenster, abgelaufenes Angebot und doppelten Annahmeklick prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
