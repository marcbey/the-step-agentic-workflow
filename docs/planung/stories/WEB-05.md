# WEB-05 – Kontakt, Standorte und Anfahrt bereitstellen

[GitHub-Issue #36](https://github.com/marcbey/the-step-agentic-workflow/issues/36)

## User Story

Als **Interessentin** möchte ich **Kontakt, Standorte und Anfahrt bereitstellen**.

**Erwarteter Nutzen:** den richtigen Ansprechpartner und Trainingsort zu erreichen.

## Einordnung

- Story-ID: [WEB-05 #36](https://github.com/marcbey/the-step-agentic-workflow/issues/36) · Epic: [E02 #2](https://github.com/marcbey/the-step-agentic-workflow/issues/2)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **5 Story Points**
- Quelle: F04, W04; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Vereinsanschrift und Trainingsort werden getrennt bezeichnet.
- [ ] **AK-02:** E-Mail, Telefon und offizielle Website werden aus geprüften zentralen Angaben ausgegeben.
- [ ] **AK-03:** Bürozeiten werden nur angezeigt, wenn der Verein sie bestätigt hat.
- [ ] **AK-04:** Kontaktformular bietet Anliegenwahl, Pflichtfeldprüfung und verständliche Versandbestätigung.
- [ ] **AK-05:** Rate Limit und Spamabwehr verhindern automatisierte Serienanfragen ohne unzugängliches Pflicht-Captcha.
- [ ] **AK-06:** Anfahrt ist ohne Drittanbieterkarte nutzbar; Google Maps lädt erst nach eigener Freigabe.

## Abhängigkeiten und Voraussetzungen

[BAS-06 #19](https://github.com/marcbey/the-step-agentic-workflow/issues/19), [GOV-01 #24](https://github.com/marcbey/the-step-agentic-workflow/issues/24)

**Vor Umsetzung zu klären:** D04. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Nur freigegebene Inhalte aus WebPage/Content::Repository und öffentlich gefilterte Fachdaten.

**Voraussichtliche Codeorte:** `app/controllers/pages_controller.rb, app/views/pages/, app/views/shared/, config/content/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Spam, Mailausfall, leere Bürozeiten und Ablehnung externer Inhalte prüfen; erneutes Absenden erzeugt keine Duplikate.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
