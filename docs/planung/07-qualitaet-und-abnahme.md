# Qualität und fachliche Abnahme

## Definition of Done pro umgesetzter Story

- Alle AKs sind erfüllt und über passende Tests, sichtbare Beispiele oder dokumentierte Fachprüfung nachgewiesen.
- Betroffene Rollen können die erlaubten Fälle ausführen; direkte fremde IDs, Dateien und Exporte sind ebenfalls geprüft.
- Fehler, leere Zustände, Wiederholung und relevante Grenzzeitpunkte führen zu verständlichem und konsistentem Verhalten.
- Notwendige Datenbankregeln, Migrationen und Jobs sind wiederholbar beziehungsweise kontrolliert ausführbar.
- Handbuch, Betriebsdokumentation und Changelog entsprechen dem neuen Funktionsstand.
- Änderungen sind im PR der Story zugeordnet und fachlich abgenommen. Ein erfolgreich angelegtes Issue und eine grüne allgemeine CI allein sind keine Fachabnahme.

## Fünf besonders wichtige Eingabeklassen

| Eingabe oder Fehler | Erwartung | Verantwortliche Stories |
|---|---|---|
| Gleichzeitiger letzter Platz, Ablauf und Blocktermin | Keine Überbuchung, keine Teilzusage, atomarer Übergang | BUC-02, BUC-06, ANG-08 |
| Geburtstag/Minderjährigkeit an Tagesgrenzen, Zeitumstellung | Korrektes Alter und lokaler Termin in Europe/Berlin | BUC-01, ANG-02, BUC-10 |
| Entzogene Familien- oder Coachbeziehung | Nächster Request und Direktdownload verweigert Zugriff | MIT-06, BUC-07, GOV-05 |
| Mail-/Queue-/Anbieterfehler und wiederholtes Ereignis | Nachholbare Auslieferung, keine doppelte fachliche Wirkung | BUC-04, REL-02, SHP-05 |
| Rechtewiderruf eines Bilds, private Datei oder alter Cache | Keine weitere öffentliche Auslieferung unzulässiger Varianten | CMS-03, MIT-07, GOV-04 |

## Prüfebenen und konkrete Freigaben

Bei späterer Umsetzung werden Fachregeln mit Minitest, Controller-/Policygrenzen mit Integrationstests und kritische Benutzerabläufe mit Capybara/Selenium geprüft. Echte Datenbankparallelität läuft gegen dateibasiertes SQLite mit getrennten Verbindungen; ein Mock von Kapazitätszählern genügt nicht. Anbieterintegrationen verwenden Sandbox und Vertragstests.

Voraussichtlicher lokaler Qualitätslauf nach Aufbau der Rails-Anwendung: `mise exec -- bin/rails test`, `mise exec -- bin/rails test:system`, `mise exec -- bin/rubocop`, `mise exec -- bin/brakeman --quiet --no-pager`, `mise exec -- bin/bundler-audit`, Inhaltsprüfung und anschließend `mise exec -- ./bin/ci`. Die konkreten Befehle werden in BAS-02 mit dem tatsächlichen Checkout fixiert. In diesem reinen Planungsrepository existieren diese Produktprüfungen noch nicht.

Das Inhaltsgate prüft veröffentlichte Pflichtinhalte, aktuelle Kontakt-/Anbieterangaben und freigegebene Kinderschutzkontakte. Sicherheitsprüfung umfasst CSRF/Origin, Tokenablauf, Sessionende, Rate-Limit bei Cachefehler und fehlende Verschlüsselungsschlüssel. Öffentliche Dateien, private Downloads und CSV werden gesondert geprüft.

Barrierefreiheit umfasst manuelle Tastatur-/Screenreader-Stichproben und automatisierte Kontrollen. Qualitätsziel ist [WCAG 2.2 AA](https://www.w3.org/TR/WCAG22/); eine automatische Prüfung ist kein vollständiger Konformitätsnachweis. Performancebudgets sind Planungsziele mit reproduzierbarem Messprofil, keine bereits gemessenen Ergebnisse.

## Abnahmeszenarien je Release

| Release | Ende-zu-Ende-Szenario | Fachlich abnehmende Rolle |
|---|---|---|
| R0 | Frischer Checkout, synthetische Datenbank, Adminlogin, CI, isoliertes Staging und Restore | Tech Lead/Betrieb |
| R1 | Elternteil findet passenden Kurs, reserviert und bestätigt, erhält Kosten/Regeln; Verwaltung ändert Termin; Coach checkt ein; Storno erlaubt Nachrücken | Kursplanung/Büro/Coach |
| R1 | Camp mit mehreren Tagen und regulärer Kursblock; letzter Platz unter Parallelität; keine falschen E-Mail-Zusagen bei Ausfall | Kursplanung/Tech Lead |
| R1 | Kinderschutz-/Anbieterprüfung, Rechtewiderruf, Datensicherung und Wiederherstellung mit Retention | Vorstand/Kinderschutz/Datenschutz/Betrieb |
| R2 | Mitgliedsantrag, Aufnahme, Familienzuordnung, Beitrag, Änderung/Kündigung und daraus folgender Vorteilsstatus | Vorstand/Büro/Kasse |
| R2 | Einsatz, Abwesenheit/Vertretung, Zeit einreichen/freigeben, Material ausgeben/zurücknehmen | Koordination/Kasse |
| R3 | Testkauf mit Mitgliederpreis, letzter Bestand, verifiziertem Zahlungsereignis und Rechnung; Teilretoure/Erstattung mit Gutscheinanteil | Shopteam/Kasse |
| R4 | Aktivierte Einzelfunktion samt Ausfall-/Widerrufspfad; Kernbuchung bleibt nutzbar | Zuständige Fachrolle |

Für jeden Release werden Stand, Datenbasis, Prüferrolle, Ergebnis und offene Restpunkte dokumentiert. Fachliche Blocker bleiben sichtbar. Rechtliche/steuerliche Angaben werden von den zuständigen Fachrollen bestätigt; diese Planung ersetzt keine solche Bestätigung.
