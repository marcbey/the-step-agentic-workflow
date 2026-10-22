# CMS-06 – Instagram-Inhalte als optionale Ergänzung integrieren

[GitHub-Issue #43](https://github.com/marcbey/the-step-agentic-workflow/issues/43)

## User Story

Als **Communitymitglied** möchte ich **Instagram-Inhalte als optionale Ergänzung integrieren**.

**Erwarteter Nutzen:** aktuelle Social-Media-Beiträge auf Wunsch zu sehen.

## Einordnung

- Story-ID: [CMS-06 #43](https://github.com/marcbey/the-step-agentic-workflow/issues/43) · Epic: [E03 #3](https://github.com/marcbey/the-step-agentic-workflow/issues/3)
- Release: **R4** · Priorität: **P2** · vorläufige Größe: **5 Story Points**
- Quelle: F02; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Standardansicht bietet einen einfachen Link zum offiziellen Account.
- [ ] **AK-02:** Ein Feed wird erst nach dokumentierter Anbieterentscheidung aktiviert.
- [ ] **AK-03:** Ohne eigene Zustimmung werden keine Social-Requests ausgelöst.
- [ ] **AK-04:** API-Ausfall und abgelaufene Anbieterberechtigung lassen einen nutzbaren Fallback.
- [ ] **AK-05:** Es werden nur freigegebene Vereinsinhalte angezeigt.
- [ ] **AK-06:** Kontozugänge und API-Secrets liegen ausschließlich im Secret Store.

## Abhängigkeiten und Voraussetzungen

[CMS-04 #41](https://github.com/marcbey/the-step-agentic-workflow/issues/41)

**Vor Umsetzung zu klären:** D06. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

WebPage und Community-Inhalte mit Action Text/Lexxy; Medien über Active Storage mit geprüften Sichtbarkeitsregeln.

**Voraussichtliche Codeorte:** `app/models/web_page.rb, app/models/community_*.rb, app/controllers/admin/, app/views/community/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Feed ohne Zustimmung, bei API-Ausfall und nach Rechtewiderruf prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
