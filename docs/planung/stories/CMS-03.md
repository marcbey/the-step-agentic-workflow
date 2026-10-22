# CMS-03 – Galerien mit Medienrechten und Widerruf verwalten

[GitHub-Issue #28](https://github.com/marcbey/the-step-agentic-workflow/issues/28)

## User Story

Als **Redaktion** möchte ich **Galerien mit Medienrechten und Widerruf verwalten**.

**Erwarteter Nutzen:** Bilder verantwortungsvoll und in guter Qualität zu veröffentlichen.

## Einordnung

- Story-ID: [CMS-03 #28](https://github.com/marcbey/the-step-agentic-workflow/issues/28) · Epic: [E03 #3](https://github.com/marcbey/the-step-agentic-workflow/issues/3)
- Release: **R1** · Priorität: **P0** · vorläufige Größe: **8 Story Points**
- Quelle: F01, F02, T01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** JPEG, PNG und WebP werden bis 10 MB und 25 Megapixel akzeptiert.
- [ ] **AK-02:** Bildfokus und Zoom erzeugen gemeinsame 4:3-Vorschauen.
- [ ] **AK-03:** Alternativtext, Credit und Rechtebeleg sind Veröffentlichungsvoraussetzung.
- [ ] **AK-04:** Aufnahmen Minderjähriger werden mit dokumentierter Freigabe und Nutzungsumfang verknüpft.
- [ ] **AK-05:** Widerruf sperrt alle betroffenen öffentlichen Varianten und startet Cache-/Storage-Bereinigung.
- [ ] **AK-06:** Nicht zugeordnete Uploads werden erst nach mindestens 24 Stunden kontrolliert bereinigt.

## Abhängigkeiten und Voraussetzungen

[BAS-03 #16](https://github.com/marcbey/the-step-agentic-workflow/issues/16), [BAS-04 #17](https://github.com/marcbey/the-step-agentic-workflow/issues/17)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

WebPage und Community-Inhalte mit Action Text/Lexxy; Medien über Active Storage mit geprüften Sichtbarkeitsregeln.

**Voraussichtliche Codeorte:** `app/models/web_page.rb, app/models/community_*.rb, app/controllers/admin/, app/views/community/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Zu große und falsch deklarierte Datei ablehnen; Widerruf in News, Team und Galerie inklusive Direktabruf prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
