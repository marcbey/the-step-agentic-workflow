# EXT-02 – Installierbare Web-App und optionale Push-Mitteilungen prüfen

[GitHub-Issue #97](https://github.com/marcbey/the-step-agentic-workflow/issues/97)

## User Story

Als **Mitglied** möchte ich **Installierbare Web-App und optionale Push-Mitteilungen prüfen**.

**Erwarteter Nutzen:** freiwillige Hinweise auf dem Mobilgerät zu erhalten.

## Einordnung

- Story-ID: [EXT-02 #97](https://github.com/marcbey/the-step-agentic-workflow/issues/97) · Epic: [E13 #13](https://github.com/marcbey/the-step-agentic-workflow/issues/13)
- Release: **R4** · Priorität: **P2** · vorläufige Größe: **8 Story Points**
- Quelle: F05; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Anwendungsmanifest und Installationshinweis funktionieren auf unterstützten Geräten.
- [ ] **AK-02:** Push wird nur nach aktiver separater Zustimmung und verfügbarer Browserfunktion angeboten.
- [ ] **AK-03:** Kategorien für Terminänderungen und freiwillige News sind getrennt wählbar.
- [ ] **AK-04:** Sperrbildschirmtexte enthalten keine Kinder- oder sensiblen Teilnehmerdaten.
- [ ] **AK-05:** Abmeldung und Gerätewechsel entziehen Push-Abonnements.
- [ ] **AK-06:** Offlineansichten speichern keine privaten Teilnehmerlisten und erzeugen keine falsche Buchungszusage.

## Abhängigkeiten und Voraussetzungen

[MIT-06 #65](https://github.com/marcbey/the-step-agentic-workflow/issues/65), [BUC-09 #55](https://github.com/marcbey/the-step-agentic-workflow/issues/55), [GOV-01 #24](https://github.com/marcbey/the-step-agentic-workflow/issues/24)

**Vor Umsetzung zu klären:** D28. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Optionale Integration hat einen klaren Anbieter-/Datenvertrag und lässt Kernabläufe bei Ausfall nutzbar.

**Voraussichtliche Codeorte:** `app/services/integrations/, app/controllers/, app/views/, test/contracts/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Nicht unterstützter Browser, abgelaufene Subscription, Logout am geteilten Gerät und Offlinebuchung prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
