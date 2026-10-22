# WEB-03 – Team und Trainerprofile veröffentlichen

[GitHub-Issue #33](https://github.com/marcbey/the-step-agentic-workflow/issues/33)

## User Story

Als **Elternteil** möchte ich **Team und Trainerprofile veröffentlichen**.

**Erwarteter Nutzen:** die Menschen und Qualifikationen hinter den Angeboten kennenzulernen.

## Einordnung

- Story-ID: [WEB-03 #33](https://github.com/marcbey/the-step-agentic-workflow/issues/33) · Epic: [E02 #2](https://github.com/marcbey/the-step-agentic-workflow/issues/2)
- Release: **R1** · Priorität: **P1** · vorläufige Größe: **3 Story Points**
- Quelle: F01, F03, T01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Aktive freigegebene Profile zeigen Name, Rolle, Steckbrief und freigegebene Qualifikationen.
- [ ] **AK-02:** Interne Zuständigkeiten und private Kontaktdaten werden nicht automatisch öffentlich.
- [ ] **AK-03:** Profilbild benötigt Alternativtext und dokumentierte Nutzungsfreigabe.
- [ ] **AK-04:** Öffentliches Profil erzeugt keine zusätzlichen Verwaltungsrechte.
- [ ] **AK-05:** Deaktivierung entfernt die Person aus öffentlichen Listen und Vorschauen.
- [ ] **AK-06:** Fehlendes Foto und lange Namen bleiben sauber darstellbar.

## Abhängigkeiten und Voraussetzungen

[BAS-03 #16](https://github.com/marcbey/the-step-agentic-workflow/issues/16), [CMS-03 #28](https://github.com/marcbey/the-step-agentic-workflow/issues/28)

**Vor Umsetzung zu klären:** Keine zusätzliche Einzelentscheidung; globale Releasegates gelten.. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Nur freigegebene Inhalte aus WebPage/Content::Repository und öffentlich gefilterte Fachdaten.

**Voraussichtliche Codeorte:** `app/controllers/pages_controller.rb, app/views/pages/, app/views/shared/, config/content/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Unveröffentlichtes Profil über Direktlink und Bild-URL prüfen; deaktivierten User aus Listen entfernen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
