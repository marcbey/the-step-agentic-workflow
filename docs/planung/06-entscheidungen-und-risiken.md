# Entscheidungen, Annahmen und Risiken

Alle nachstehenden Entscheidungen sind **offen**, bis die zuständige Rolle sie dokumentiert hat. Die vorgeschlagene Rolle ist keine bereits zugesagte persönliche Zuständigkeit. Die Planung ist vollständig ausgearbeitet; eine offene Fachentscheidung macht die betroffene Story noch nicht umsetzungsbereit. Bestätigung bedeutet hier fachliche Klärung im späteren Projekt und keine zusätzliche Erlaubnis, die angeforderte Planung anzulegen.

| ID | Entscheidung | Planungsvorschlag / benötigte Evidenz | Zuständige Rolle | Stories | Spätester Punkt |
|---|---|---|---|---|---|
| D01 | Codeübernahme statt Fork oder Neubau | Selektiv übernehmen; Codebestand zuerst inventarisieren | Tech Lead | BAS-01 | vor BAS-02 |
| D02 | Neue Zielumgebung, Verantwortliche, Backup-/Ausfallziele | Eigene Umgebung; RPO 24 h, RTO 4 h als Planungsziele bestätigen | Betrieb/Vorstand | BAS-04 REL-02 | vor erstem Stagingdeploy |
| D03 | Tatsächliche Kinderschutzkontakte und Konzeptfreigabe | Internen und externen Kontakt schriftlich bestätigen | Kinderschutz/Vorstand | WEB-04 GOV-02 | vor öffentlichem Start |
| D04 | Anliegenempfänger, Bürozeiten und Kontaktkanäle | Geschäftliche Ziele bestätigen; keine privaten Kontakte erfinden | Vereinsbüro | WEB-05 KOM-01 EXT-05 | vor Kontaktformular |
| D05 | Gültige öffentliche Vereinsdokumente | Aktuelle ununterschriebene beziehungsweise bereinigte Veröffentlichungsfassungen liefern | Vorstand | WEB-07 | vor Veröffentlichung |
| D06 | Instagram-Modell und Accountverantwortung | Zunächst einfacher Link; Feed nur bei bestätigtem Bedarf | Redaktion | CMS-06 | vor Feedanbindung |
| D07 | Reales Angebotsinventar, Alter, Level, Kapazitäten und Preise | Vereinswerte übernehmen, Muster aussondern | Kursplanung | ANG-01 | vor öffentlicher Buchung |
| D08 | Geburtstagsangebote, Freigabe und Stornoregel | Zweistufige Anfrage/Angebot statt ungeprüfter Sofortzusage | Kursplanung | ANG-05 | vor verbindlichem Angebot |
| D09 | Schutzregeln, Verzicht und Leihgebühren | 5 Euro je Kategorie aus Referenz bestätigen; Verzicht fachlich prüfen | Kursplanung/Kinderschutz | ANG-07 | vor Buchungsformular |
| D10 | Regelmäßige Kurse: Block, Einzeltermin oder beides | Explizite Einheiten, keine stillen Teilbuchungen | Kursplanung/Kasse | ANG-08 | vor Serienbuchung |
| D11 | Reservierungsdauer und SQLite-Kapazitätsvertrag | Maximal 60 Minuten bis Kursbeginn; echten Konkurrenztest verlangen | Tech Lead/Kursplanung | BUC-02 | vor Buchungsfreigabe |
| D12 | Mitgliederpreise und Rabattkombination | R1 Selbstauskunft mit Prüfung, R2 zentrale Statusprüfung | Vorstand/Kasse | BUC-03 MIT-05 SHP-03 | vor Preisaktivierung |
| D13 | Storno-, Umbuchungs- und Erstattungsbedingungen | Einheitliche veröffentlichte Regeln pro Angebotsart | Vorstand/Kasse | BUC-05 | vor verbindlicher Buchung |
| D14 | Wartelistenrang und Nachrückfrist | FIFO, 24 h begrenzt durch Buchungsschluss; Ausnahmen nur auditiert | Kursplanung | BUC-06 | vor Warteliste |
| D15 | Newsletteranbieter und Verantwortlichkeit | Double-Opt-in, gesonderte Einwilligung, keine Buchungsdatenübernahme | Redaktion/Datenschutz | KOM-02 | vor Newsletterstart |
| D16 | Rechnungs-/Steuermodell und erforderliche Formate | Steuerberatung bestätigt Pflichtangaben, Formate und Korrekturprozess | Kasse/Steuerberatung | FIN-01 FIN-02 SHP-08 | vor automatischem Beleg |
| D17 | Mitgliedschaftsarten, Beiträge, Fristen und SEPA | Gültige Satzung/Beitragsordnung als einzige Fachquelle | Vorstand/Kasse | MIT-01 MIT-02 MIT-04 FIN-03 | vor Antrags-/Beitragsstart |
| D18 | Online-Zahlung für Kursangebote | R1 Zahlung vor Ort; Ausbau nur nach Anbieter-/Prozessentscheidung | Vorstand/Kasse | FIN-05 | vor Kurszahlungsintegration |
| D19 | Nachweis und Entzug von Familienbeziehungen | Explizite Bestätigung statt E-Mail-/Namensabgleich | Vereinsbüro/Datenschutz | MIT-06 | vor Familienportal |
| D20 | Trainerbedarf, Qualifikationen und Vertretungsregeln | Betreuungszahl und Konfliktregeln je Angebot bestätigen | Kurskoordination | OPS-01 OPS-05 | vor Einsatzautomatisierung |
| D21 | Zeitarten, Pausen, Freigabe und Abrechnungsexport | Fachregeln und Vier-Augen-Verfahren bestätigen | Personal/Kasse | OPS-03 OPS-04 | vor Zeiterfassung |
| D22 | Materialverfügbarkeit und Reservierungswirkung | Bestand und Wartung erfassen; harte Buchungssperre nur nach Fachentscheidung | Materialkoordination | OPS-07 | vor Bestandsbindung |
| D23 | Händler, Shoparchitektur, PSP, Versand und Rückgabe | Integriert vs. gehostet anhand echter Betriebsverantwortung entscheiden | Vorstand/Shopteam | SHP-01 SHP-05 SHP-06 SHP-08 | vor Checkoutbau |
| D24 | Wert-/Leistungsgutschein, Restwert und Gültigkeit | Fachlich und steuerlich freigegebenes Gutscheinmodell | Kasse/Shopteam | SHP-07 SHP-08 | vor Gutscheinverkauf |
| D25 | Fristen und Rechtsgrundlagen je Datenklasse | Referenzfristen bestätigen; Belege/Mitglieder/Zeiten getrennt behandeln | Datenschutz/Kasse | GOV-03 GOV-04 | vor Speicherung neuer Datenklassen |
| D26 | Migration echter Daten und Umschaltverantwortung | Selektiver Trockenlauf, geprüfte Zuordnung und dokumentierter Rückfall | Projektleitung/Betrieb | REL-01 | vor Import echter Daten |
| D27 | Spendenempfang und Bescheinigungsprozess | Berechtigung und Buchhaltungsablauf vor Aktivierung bestätigen | Vorstand/Kasse | EXT-01 | vor Spendenfunktion |
| D28 | Konkreter Nutzen von PWA/Push und Vereins-App | Eigenständige Nutzenentscheidung; externe App zuerst benennen | Vorstand/Team | EXT-02 EXT-09 | vor Integrationsarbeit |
| D29 | Bewertungsregeln und Moderationsverantwortung | Teilnahmebezug, Schutz Minderjähriger und Löschwege vorab festlegen | Community/Kinderschutz | EXT-03 | vor öffentlicher Bewertung |
| D30 | Empfehlungsvorteile und Missbrauchsgrenzen | Budgetierte beschlossene Regel ohne automatische Fremdkontaktaufnahme | Vorstand/Kasse | EXT-06 | vor Werbeprogramm |
| D31 | Wetteranbieter, Aktualität und Budget | Nur Information; Kursentscheidung bleibt bei der Planung | Kursplanung/Betrieb | EXT-08 | vor Wetterintegration |

## Wesentliche Risiken und Gegenmaßnahmen

| Risiko | Auswirkung | Gegenmaßnahme und Nachweis |
|---|---|---|
| Historische Dokumente widersprechen aktuellem Code | Rückbau vorhandener Funktionen oder falsche Scopeannahmen | BAS-01 inventarisiert; Live/Code/Tests werden gegen ältere Texte abgeglichen |
| Gleichzeitige letzte-Platz-Anfragen | Überbuchung und Sicherheitsprobleme | BUC-02/ANG-08 mit realer SQLite-Parallelität und Fehlerfällen |
| Zweite Person beansprucht ein Kind | Unberechtigter Zugriff auf Teilnehmerdaten | Explizite Familienfreigabe, negative ID-Tests, sofortiger Entzug |
| Mail/Worker fällt aus | Reservierung/Erinnerung wird nicht wirksam kommuniziert | Transaktionale Outbox, Wiederholung, Überwachung und operative Wiederholung |
| Bilder ohne ausreichende Rechte | Unzulässige Veröffentlichung, besonders bei Kindern | Rechtebeleg, Veröffentlichungstor, wirksamer Widerruf aller Varianten |
| Ungeprüfte Kontakte oder Rechtstexte | Fehlleitung oder falsche Transparenz | Blockierende Inhaltsgates und benannte fachliche Verantwortungen |
| Gemeinsamer Produktivserver/Volume mit Referenz | Bestehender Betrieb wird überschrieben | Eigene Zielumgebung und Service-/Volumenidentitäten |
| Backup stellt gelöschte Daten wieder her | Datenlebenszyklus wird unterlaufen | Isolierter Restore, sofortige Retention und kein ungeprüfter Rückimport |
| Shopanbieter oder Steuerentscheidung fehlt | Ungeplante Integration/Abrechnung | SHP-01/FIN-01 sind explizite Voraussetzungen des Handelsstarts |
| Gesamtumfang wird als erster Release behandelt | Zu später erster Nutzen und zu viel gleichzeitige Arbeit | Fünf Releases, fachliche Epics und begrenzte parallele Umsetzung |
| Punkte werden als Terminversprechen gelesen | Fehlplanung bei unbekannter Kapazität | Relative Schätzung; Forecast erst nach mindestens zwei realen Umsetzungstakten |

Keine Zugangsdaten, Schlüssel, Teilnehmerdaten, Finanzbestände oder vertraulichen Kinderschutzfälle gehören in öffentliche Issues. GitHub enthält Planung und synthetische Testfälle. Personenbezogene Betriebsfälle verbleiben im dafür vorgesehenen geschützten System.
