# BAS-01 – Referenzbestand und Wiederverwendungsstrategie abgleichen

[GitHub-Issue #14](https://github.com/marcbey/the-step-agentic-workflow/issues/14)

## User Story

Als **Entwicklung** möchte ich **Referenzbestand und Wiederverwendungsstrategie abgleichen**.

**Erwarteter Nutzen:** eine nachvollziehbare Ausgangsbasis ohne veraltete Prototypannahmen.

## Einordnung

- Story-ID: [BAS-01 #14](https://github.com/marcbey/the-step-agentic-workflow/issues/14) · Epic: [E01 #1](https://github.com/marcbey/the-step-agentic-workflow/issues/1)
- Release: **R0** · Priorität: **P0** · vorläufige Größe: **3 Story Points**
- Quelle: T01, W01; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Referenzcommit b82d07f387b35836b273800b3d7fd169b6a1a145 und Liveabruf vom 22.10.2026 sind dokumentiert.
- [ ] **AK-02:** Funktionen werden als übernehmen, anpassen oder neu entwickeln eingestuft.
- [ ] **AK-03:** Code und Liveinhalt haben bei Widersprüchen Vorrang vor älteren README-Passagen.
- [ ] **AK-04:** Buchung, Zahlungsstatus und Community werden anhand realer Modelle und Tests inventarisiert.
- [ ] **AK-05:** Übernahme enthält weder Zugangsdaten noch Datenbanken oder echte Teilnehmerdaten.
- [ ] **AK-06:** Ein Architekturentscheid vergleicht selektive Codeübernahme, vollständigen Fork und Neubau und begründet die Auswahl.

## Abhängigkeiten und Voraussetzungen

Keine fachliche Vorgängerstory.

**Vor Umsetzung zu klären:** D01. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Rails-Boot, User/Session, zentrale Design-Tokens und Layout-Partials; kein zweites Identitätssystem.

**Voraussichtliche Codeorte:** `config/, Gemfile, .mise.toml, bin/ci, app/models/user.rb, app/assets/stylesheets/, app/views/layouts/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Inventar gegen Gemfile.lock, Routen und mindestens Buchungs-/User-/Community-Modelle prüfen; veraltete README-Aussagen sichtbar kennzeichnen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
