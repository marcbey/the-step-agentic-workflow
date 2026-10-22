# EXT-09 – Anbindung einer externen Vereins-App spezifizieren

[GitHub-Issue #104](https://github.com/marcbey/the-step-agentic-workflow/issues/104)

## User Story

Als **Vereinskoordination** möchte ich **Anbindung einer externen Vereins-App spezifizieren**.

**Erwarteter Nutzen:** Datenpflege zwischen Website und Vereins-App zu vermeiden.

## Einordnung

- Story-ID: [EXT-09 #104](https://github.com/marcbey/the-step-agentic-workflow/issues/104) · Epic: [E13 #13](https://github.com/marcbey/the-step-agentic-workflow/issues/13)
- Release: **R4** · Priorität: **P2** · vorläufige Größe: **5 Story Points**
- Quelle: F05; siehe [Quellenregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/02-quellen-und-abdeckung.md).
- Stand: geplant, nicht implementiert. Punkte sind relative Größen, keine Tage oder Zusage.

## Umfang und Akzeptanzkriterien

Die folgenden Kriterien bilden den vollständigen Umfang dieser Story; jeder Punkt benötigt einen prüfbaren Nachweis.

- [ ] **AK-01:** Konkrete Ziel-App und ihr benötigter Nutzen werden vor Schnittstellenbau benannt.
- [ ] **AK-02:** Führendes System und erlaubte Synchronisationsrichtung sind pro Datenart festgelegt.
- [ ] **AK-03:** Zugriff nutzt minimale Berechtigungen und widerrufbare Zugangsmittel.
- [ ] **AK-04:** Keine Teilnehmer- und Kinderdaten werden ohne begründeten Bedarf synchronisiert.
- [ ] **AK-05:** Fehler, Wiederholungen und Dubletten sind im Schnittstellenvertrag geregelt.
- [ ] **AK-06:** Ein isolierter Test mit synthetischen Daten belegt den vereinbarten Ablauf.

## Abhängigkeiten und Voraussetzungen

[MIT-06 #65](https://github.com/marcbey/the-step-agentic-workflow/issues/65), [GOV-04 #89](https://github.com/marcbey/the-step-agentic-workflow/issues/89)

**Vor Umsetzung zu klären:** D28. Details, Zuständigkeit und spätester Entscheidungspunkt stehen im [Entscheidungsregister](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/06-entscheidungen-und-risiken.md). Offene Entscheidungen blockieren den betroffenen Umsetzungsteil, nicht die übrige Planung.

## Technische Leitplanken

Optionale Integration hat einen klaren Anbieter-/Datenvertrag und lässt Kernabläufe bei Ausfall nutzbar.

**Voraussichtliche Codeorte:** `app/services/integrations/, app/controllers/, app/views/, test/contracts/`. Die Zielpfade sind Planvorschläge für das neue Repository und werden im Referenzabgleich BAS-01 konkretisiert; sie sind kein behaupteter vorhandener Code.

**Gezielter Prüffall:** Doppeltes Ereignis, widerrufenen Zugriff und abweichende Mitgliedschaftsstände im Vertragsbeispiel prüfen.

## Umsetzungsschritte

- [ ] Abhängigkeiten, Fachwerte und betroffene Rollen mit dem aktuellen Konzept abgleichen.
- [ ] Die oben genannten positiven Fälle und Fehler-/Grenzfälle als passende Fach-, Integrations- oder Systemprüfungen konkretisieren.
- [ ] Kleinsten unabhängig abnehmbaren Funktionsumfang einschließlich Fehlerrückmeldungen umsetzen.
- [ ] Berechtigungen und relevante Daten-/Datei-/Mailzugriffe auch mit manipulierten Direktrequests prüfen.
- [ ] Handbuch, nötige Betriebsangaben und Changelog im selben PR aktualisieren.
- [ ] AK-Nachweise verlinken, fachliche Abnahme einholen und erst dann auf Done setzen.

Es gelten zusätzlich die [gemeinsamen Qualitäts- und Abnahmeregeln](https://github.com/marcbey/the-step-agentic-workflow/blob/main/docs/planung/07-qualitaet-und-abnahme.md). Die Anlage dieses Issues erfüllt noch kein AK der Produktumsetzung.
