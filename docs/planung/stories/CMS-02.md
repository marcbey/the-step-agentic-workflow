# CMS-02 – News und Vereinsberichte veröffentlichen

[GitHub-Issue #29](https://github.com/marcbey/the-step-agentic-workflow/issues/29)

## User Story

Als **Redaktion** möchte ich **News und Vereinsberichte veröffentlichen**.

**Erwarteter Nutzen:** aktuelle Vereinsnachrichten und Rückblicke zu teilen.

## Einordnung

- Story-ID: [CMS-02 #29](https://github.com/marcbey/the-step-agentic-workflow/issues/29) · Epic: [E03 #3](https://github.com/marcbey/the-step-agentic-workflow/issues/3)
- Release: **R1** · Priorität: **P1** · vorläufige Größe: **5 Story Points**
- Quelle: F01, F02, F03; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** News zeigen Titel, Datum, Kurztext und strukturierten Inhalt.
- [ ] **AK-02:** Entwurf, Veröffentlichungstermin und Archiv sind pflegbar.
- [ ] **AK-03:** Startseite verwendet ausgewählte veröffentlichte Beiträge.
- [ ] **AK-04:** Kategorien unterstützen Vereinsleben, Kurse und Veranstaltungen.
- [ ] **AK-05:** Bilder und Galerieverweise verwenden zentrale Medienrechte.
- [ ] **AK-06:** Fehlende Beiträge führen zu einem verständlichen leeren Zustand.

## Abhängigkeiten und Voraussetzungen

[CMS-01 #20](https://github.com/marcbey/the-step-agentic-workflow/issues/20), [CMS-03 #28](https://github.com/marcbey/the-step-agentic-workflow/issues/28)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

WebPage und Community-Inhalte mit Action Text/Lexxy; Medien über Active Storage mit geprüften Sichtbarkeitsregeln.

**Voraussichtliche Codeorte:** `app/models/web_page.rb, app/models/community_*.rb, app/controllers/admin/, app/views/community/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Geplanter Beitrag darf vor Termin nicht öffentlich werden; Archivierung muss Startseite und Suche aktualisieren.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
