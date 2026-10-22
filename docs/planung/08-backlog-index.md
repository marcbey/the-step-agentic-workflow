# Backlogindex

[Projektboard](https://github.com/users/marcbey/projects/4) · [Maschinenlesbarer Plan](backlog.json)

## [E01](https://github.com/marcbey/the-step-agentic-workflow/issues/1) – Technische Basis und Designsystem

| Story | Release | Priorität | Punkte | Abhängigkeiten |
|---|---|---|---:|---|
| [BAS-01 – Referenzbestand und Wiederverwendungsstrategie abgleichen](https://github.com/marcbey/the-step-agentic-workflow/issues/14) | R0 | P0 | 3 | – |
| [BAS-02 – Rails-Anwendung und reproduzierbare CI vorbereiten](https://github.com/marcbey/the-step-agentic-workflow/issues/15) | R0 | P0 | 5 | BAS-01 |
| [BAS-03 – Konten, Rollen und Zuständigkeiten trennen](https://github.com/marcbey/the-step-agentic-workflow/issues/16) | R0 | P0 | 8 | BAS-02 |
| [BAS-04 – Isoliertes Staging und wiederherstellbares Deployment planen](https://github.com/marcbey/the-step-agentic-workflow/issues/17) | R0 | P0 | 8 | BAS-02 |
| [BAS-05 – Bestehendes TheStep-Design als Komponentenbasis übernehmen](https://github.com/marcbey/the-step-agentic-workflow/issues/18) | R0 | P0 | 5 | BAS-01, BAS-02 |
| [BAS-06 – Navigation und zugängliche Grundlayouts erstellen](https://github.com/marcbey/the-step-agentic-workflow/issues/19) | R0 | P0 | 5 | BAS-05 |

## [E02](https://github.com/marcbey/the-step-agentic-workflow/issues/2) – Öffentliche Website und Vereinsinformationen

| Story | Release | Priorität | Punkte | Abhängigkeiten |
|---|---|---|---:|---|
| [WEB-01 – Startseite mit aktuellen Einstiegen gestalten](https://github.com/marcbey/the-step-agentic-workflow/issues/31) | R1 | P0 | 5 | BAS-06, ANG-03, CMS-02, EVT-01 |
| [WEB-02 – Verein, Geschichte und Abgrenzung zum Stuttpark darstellen](https://github.com/marcbey/the-step-agentic-workflow/issues/32) | R1 | P0 | 3 | BAS-06, CMS-01 |
| [WEB-03 – Team und Trainerprofile veröffentlichen](https://github.com/marcbey/the-step-agentic-workflow/issues/33) | R1 | P1 | 3 | BAS-03, CMS-03 |
| [WEB-04 – Kinderschutzseite und verlässliche Kontaktwege bereitstellen](https://github.com/marcbey/the-step-agentic-workflow/issues/35) | R1 | P0 | 5 | CMS-01, WEB-07 |
| [WEB-05 – Kontakt, Standorte und Anfahrt bereitstellen](https://github.com/marcbey/the-step-agentic-workflow/issues/36) | R1 | P0 | 5 | BAS-06, GOV-01 |
| [WEB-06 – Service, Sicherheit und häufige Fragen pflegen](https://github.com/marcbey/the-step-agentic-workflow/issues/37) | R1 | P0 | 3 | ANG-01, CMS-01 |
| [WEB-07 – Versionierte öffentliche Downloads bereitstellen](https://github.com/marcbey/the-step-agentic-workflow/issues/34) | R1 | P0 | 5 | CMS-01 |
| [WEB-08 – Sponsoren und Kooperationen sichtbar machen](https://github.com/marcbey/the-step-agentic-workflow/issues/38) | R1 | P1 | 3 | CMS-01, WEB-05 |
| [WEB-09 – Ehrenamt, Jobs, Praktikum und FSJ vorstellen](https://github.com/marcbey/the-step-agentic-workflow/issues/39) | R1 | P1 | 3 | CMS-01, WEB-05 |
| [WEB-10 – Öffentliche Suche und Suchmaschinenbasis anbieten](https://github.com/marcbey/the-step-agentic-workflow/issues/40) | R1 | P1 | 5 | CMS-01, ANG-03, EVT-01 |

## [E03](https://github.com/marcbey/the-step-agentic-workflow/issues/3) – Redaktion, Community und Medien

| Story | Release | Priorität | Punkte | Abhängigkeiten |
|---|---|---|---:|---|
| [CMS-01 – Redaktionelle Seiten mit Vorschau und Freigabe verwalten](https://github.com/marcbey/the-step-agentic-workflow/issues/20) | R1 | P0 | 5 | BAS-03, BAS-05 |
| [CMS-02 – News und Vereinsberichte veröffentlichen](https://github.com/marcbey/the-step-agentic-workflow/issues/29) | R1 | P1 | 5 | CMS-01, CMS-03 |
| [CMS-03 – Galerien mit Medienrechten und Widerruf verwalten](https://github.com/marcbey/the-step-agentic-workflow/issues/28) | R1 | P0 | 8 | BAS-03, BAS-04 |
| [CMS-04 – Videos und externe Medien mit Zustimmung anzeigen](https://github.com/marcbey/the-step-agentic-workflow/issues/41) | R1 | P1 | 5 | CMS-03, GOV-01 |
| [CMS-05 – Pressebereich und freigegebene Materialien bereitstellen](https://github.com/marcbey/the-step-agentic-workflow/issues/42) | R1 | P1 | 3 | CMS-01, CMS-03, WEB-05 |
| [CMS-06 – Instagram-Inhalte als optionale Ergänzung integrieren](https://github.com/marcbey/the-step-agentic-workflow/issues/43) | R4 | P2 | 5 | CMS-04 |

## [E04](https://github.com/marcbey/the-step-agentic-workflow/issues/4) – Skateangebote und Terminplanung

| Story | Release | Priorität | Punkte | Abhängigkeiten |
|---|---|---|---:|---|
| [ANG-01 – Angebotsarten und veröffentlichbare Angebotsdaten modellieren](https://github.com/marcbey/the-step-agentic-workflow/issues/21) | R1 | P0 | 8 | BAS-02, CMS-01 |
| [ANG-02 – Serien, Ausnahmen und Ferien im Kurskalender planen](https://github.com/marcbey/the-step-agentic-workflow/issues/22) | R1 | P0 | 8 | ANG-01 |
| [ANG-03 – Angebotsübersicht und Angebotsdetails bereitstellen](https://github.com/marcbey/the-step-agentic-workflow/issues/27) | R1 | P0 | 5 | ANG-01, ANG-02, BUC-02 |
| [ANG-04 – Camps und mehrtägige Workshops als Buchungseinheit führen](https://github.com/marcbey/the-step-agentic-workflow/issues/44) | R1 | P0 | 5 | ANG-01, ANG-02 |
| [ANG-05 – Geburtstage vom Wunschtermin bis zur Bestätigung abwickeln](https://github.com/marcbey/the-step-agentic-workflow/issues/46) | R1 | P0 | 8 | ANG-01, WEB-05, KOM-01 |
| [ANG-06 – Schul-AGs, Gruppen und Firmenevents als Anfrage anbieten](https://github.com/marcbey/the-step-agentic-workflow/issues/47) | R2 | P1 | 5 | ANG-01, WEB-05, KOM-01 |
| [ANG-07 – Leihmaterial und Ausrüstung im Angebot berücksichtigen](https://github.com/marcbey/the-step-agentic-workflow/issues/23) | R1 | P0 | 5 | ANG-01 |
| [ANG-08 – Regelmäßige Kurse und Kursblöcke buchbar machen](https://github.com/marcbey/the-step-agentic-workflow/issues/48) | R1 | P0 | 8 | ANG-02, BUC-01, BUC-02 |

## [E05](https://github.com/marcbey/the-step-agentic-workflow/issues/5) – Buchung und Teilnehmerbetrieb

| Story | Release | Priorität | Punkte | Abhängigkeiten |
|---|---|---|---:|---|
| [BUC-01 – Gastbuchung mit Minderjährigen- und Einwilligungslogik anbieten](https://github.com/marcbey/the-step-agentic-workflow/issues/25) | R1 | P0 | 8 | ANG-01, ANG-07, GOV-01 |
| [BUC-02 – Plätze atomar reservieren und per E-Mail bestätigen](https://github.com/marcbey/the-step-agentic-workflow/issues/26) | R1 | P0 | 13 | BUC-01, BAS-02 |
| [BUC-03 – Preise und Mitgliedervorteile historisch korrekt berechnen](https://github.com/marcbey/the-step-agentic-workflow/issues/49) | R1 | P0 | 5 | BUC-02 |
| [BUC-04 – Buchungse-Mails und Versandwiederholung zuverlässig ausliefern](https://github.com/marcbey/the-step-agentic-workflow/issues/50) | R1 | P0 | 8 | BUC-02, BAS-04 |
| [BUC-05 – Selbststorno, Umbuchung und Angebotsabsage durchführen](https://github.com/marcbey/the-step-agentic-workflow/issues/51) | R1 | P0 | 8 | BUC-02, BUC-04 |
| [BUC-06 – Warteliste mit befristetem Nachrückangebot anbieten](https://github.com/marcbey/the-step-agentic-workflow/issues/52) | R1 | P0 | 8 | BUC-02, BUC-04, BUC-05 |
| [BUC-07 – Teilnehmerlisten, Check-in und Anwesenheit je Termin führen](https://github.com/marcbey/the-step-agentic-workflow/issues/53) | R1 | P0 | 8 | BUC-02, BAS-03, ANG-04 |
| [BUC-08 – Manuelle Buchungen und sichere Exporte ermöglichen](https://github.com/marcbey/the-step-agentic-workflow/issues/54) | R1 | P0 | 5 | BUC-02, BUC-03, BUC-07 |
| [BUC-09 – Kurs- und Wettermitteilungen gezielt versenden](https://github.com/marcbey/the-step-agentic-workflow/issues/55) | R1 | P0 | 5 | BUC-04, BUC-07 |
| [BUC-10 – Automatische Erinnerungen zustandsabhängig versenden](https://github.com/marcbey/the-step-agentic-workflow/issues/56) | R1 | P1 | 5 | BUC-04, BUC-07 |

## [E06](https://github.com/marcbey/the-step-agentic-workflow/issues/6) – Veranstaltungen und Kommunikation

| Story | Release | Priorität | Punkte | Abhängigkeiten |
|---|---|---|---:|---|
| [EVT-01 – Veranstaltungskalender und Eventdetails veröffentlichen](https://github.com/marcbey/the-step-agentic-workflow/issues/30) | R1 | P0 | 5 | CMS-01, ANG-02 |
| [EVT-02 – Online-Anmeldung für Veranstaltungen integrieren](https://github.com/marcbey/the-step-agentic-workflow/issues/57) | R1 | P1 | 5 | EVT-01, BUC-02, BUC-04 |
| [KOM-01 – Kontaktanliegen und Gruppenanfragen zustellen](https://github.com/marcbey/the-step-agentic-workflow/issues/45) | R1 | P0 | 5 | WEB-05, BAS-03 |
| [KOM-02 – Newsletter mit bestätigter Anmeldung anbieten](https://github.com/marcbey/the-step-agentic-workflow/issues/58) | R2 | P1 | 5 | GOV-01 |

## [E07](https://github.com/marcbey/the-step-agentic-workflow/issues/7) – Rechnungen und Zahlungsverwaltung

| Story | Release | Priorität | Punkte | Abhängigkeiten |
|---|---|---|---:|---|
| [FIN-01 – Rechnungen und Korrekturbelege automatisch erstellen](https://github.com/marcbey/the-step-agentic-workflow/issues/60) | R2 | P0 | 8 | BUC-03, BUC-04, GOV-02 |
| [FIN-02 – Zahlungen vor Ort und Forderungsstatus nachvollziehbar führen](https://github.com/marcbey/the-step-agentic-workflow/issues/61) | R1 | P0 | 5 | BUC-03, BAS-03 |
| [FIN-03 – Beitragsläufe und Finanzexporte vorbereiten](https://github.com/marcbey/the-step-agentic-workflow/issues/64) | R2 | P0 | 8 | MIT-01, MIT-02, FIN-01 |
| [FIN-04 – Rechnungen und Buchungsbelege im eigenen Portal anzeigen](https://github.com/marcbey/the-step-agentic-workflow/issues/66) | R2 | P1 | 5 | FIN-01, MIT-06 |
| [FIN-05 – Online-Zahlungsmodell für Angebote entscheiden](https://github.com/marcbey/the-step-agentic-workflow/issues/67) | R3 | P1 | 5 | FIN-01, FIN-02 |

## [E08](https://github.com/marcbey/the-step-agentic-workflow/issues/8) – Mitgliedschaft, Familie und Selbstservice

| Story | Release | Priorität | Punkte | Abhängigkeiten |
|---|---|---|---:|---|
| [MIT-01 – Mitgliedschaft, Beiträge und Vorteile verständlich erklären](https://github.com/marcbey/the-step-agentic-workflow/issues/62) | R2 | P0 | 3 | WEB-02, WEB-07 |
| [MIT-02 – Online-Mitgliedsantrag und Aufnahme bearbeiten](https://github.com/marcbey/the-step-agentic-workflow/issues/63) | R2 | P0 | 8 | MIT-01, BAS-03, GOV-01 |
| [MIT-03 – Mitgliederdaten und Änderungen im Selbstservice pflegen](https://github.com/marcbey/the-step-agentic-workflow/issues/68) | R2 | P1 | 5 | MIT-02, MIT-06 |
| [MIT-04 – Kündigungen und Mitgliedschaftswechsel abwickeln](https://github.com/marcbey/the-step-agentic-workflow/issues/69) | R2 | P0 | 5 | MIT-02, FIN-03 |
| [MIT-05 – Mitgliedervorteile zentral und zeitabhängig prüfen](https://github.com/marcbey/the-step-agentic-workflow/issues/70) | R2 | P0 | 5 | MIT-02, MIT-04, BUC-03 |
| [MIT-06 – Mein TheStep und freigegebene Familienbeziehungen bereitstellen](https://github.com/marcbey/the-step-agentic-workflow/issues/65) | R2 | P0 | 8 | BAS-03, MIT-02, BUC-02 |
| [MIT-07 – Geschützte Vereinsdokumente im Portal bereitstellen](https://github.com/marcbey/the-step-agentic-workflow/issues/71) | R2 | P1 | 3 | MIT-06, WEB-07 |
| [MIT-08 – Elternhilfe und Ehrenamtseinsätze organisieren](https://github.com/marcbey/the-step-agentic-workflow/issues/72) | R2 | P1 | 5 | MIT-06, EVT-01, BUC-04 |

## [E09](https://github.com/marcbey/the-step-agentic-workflow/issues/9) – Trainer- und Mitarbeiterportal

| Story | Release | Priorität | Punkte | Abhängigkeiten |
|---|---|---|---:|---|
| [OPS-01 – Trainereinsätze und Zuständigkeiten planen](https://github.com/marcbey/the-step-agentic-workflow/issues/73) | R2 | P0 | 8 | BUC-07, BAS-03 |
| [OPS-02 – Persönlichen Mitarbeiterkalender und Kursbesetzung anzeigen](https://github.com/marcbey/the-step-agentic-workflow/issues/74) | R2 | P1 | 5 | OPS-01 |
| [OPS-03 – Arbeits- und Ehrenamtsstunden erfassen](https://github.com/marcbey/the-step-agentic-workflow/issues/75) | R2 | P0 | 5 | BAS-03, OPS-01 |
| [OPS-04 – Stunden prüfen, freigeben und exportieren](https://github.com/marcbey/the-step-agentic-workflow/issues/76) | R2 | P0 | 5 | OPS-03 |
| [OPS-05 – Abwesenheit, Urlaub und Vertretung bearbeiten](https://github.com/marcbey/the-step-agentic-workflow/issues/77) | R2 | P1 | 5 | OPS-01, OPS-02 |
| [OPS-06 – Interne News und Mitarbeiterdokumente bereitstellen](https://github.com/marcbey/the-step-agentic-workflow/issues/78) | R2 | P1 | 5 | BAS-03, CMS-01, MIT-07 |
| [OPS-07 – Materialbestand, Ausgabe und Wartung verwalten](https://github.com/marcbey/the-step-agentic-workflow/issues/79) | R2 | P1 | 8 | ANG-07, BUC-07 |

## [E10](https://github.com/marcbey/the-step-agentic-workflow/issues/10) – Shop, Bestellungen und Gutscheine

| Story | Release | Priorität | Punkte | Abhängigkeiten |
|---|---|---|---:|---|
| [SHP-01 – Handelsmodell und Shopschnittstelle entscheiden](https://github.com/marcbey/the-step-agentic-workflow/issues/80) | R3 | P0 | 5 | MIT-05, FIN-01, GOV-02 |
| [SHP-02 – Produkte, Varianten und Vereinskollektion darstellen](https://github.com/marcbey/the-step-agentic-workflow/issues/81) | R3 | P1 | 5 | SHP-01, CMS-03 |
| [SHP-03 – Mitgliederpreise sicher im Shop anwenden](https://github.com/marcbey/the-step-agentic-workflow/issues/82) | R3 | P0 | 5 | SHP-02, MIT-05 |
| [SHP-04 – Warenkorb und bestandsfeste Reservierung umsetzen](https://github.com/marcbey/the-step-agentic-workflow/issues/83) | R3 | P0 | 8 | SHP-02, SHP-03 |
| [SHP-05 – Gehosteten Checkout und Zahlungsrückmeldungen integrieren](https://github.com/marcbey/the-step-agentic-workflow/issues/84) | R3 | P0 | 13 | SHP-04, FIN-01 |
| [SHP-06 – Bestellungen, Versand, Abholung und Retouren bearbeiten](https://github.com/marcbey/the-step-agentic-workflow/issues/85) | R3 | P0 | 8 | SHP-05 |
| [SHP-07 – Digitale Geschenkgutscheine ausgeben und einlösen](https://github.com/marcbey/the-step-agentic-workflow/issues/86) | R3 | P0 | 8 | SHP-05, FIN-01 |
| [SHP-08 – Shopbedingungen und Rechnungskette freigeben](https://github.com/marcbey/the-step-agentic-workflow/issues/87) | R3 | P0 | 5 | SHP-01, SHP-05, SHP-06, SHP-07, GOV-02 |

## [E11](https://github.com/marcbey/the-step-agentic-workflow/issues/11) – Datenschutz, Sicherheit und Qualität

| Story | Release | Priorität | Punkte | Abhängigkeiten |
|---|---|---|---:|---|
| [GOV-01 – Einwilligungen, Drittinhalte und Datenschutzeinstellungen trennen](https://github.com/marcbey/the-step-agentic-workflow/issues/24) | R1 | P0 | 5 | BAS-02 |
| [GOV-02 – Rechtstexte und Anbieterangaben kontrolliert übernehmen](https://github.com/marcbey/the-step-agentic-workflow/issues/59) | R1 | P0 | 5 | CMS-01, GOV-01 |
| [GOV-03 – Datenaufbewahrung und automatische Bereinigung umsetzen](https://github.com/marcbey/the-step-agentic-workflow/issues/88) | R1 | P0 | 8 | BUC-02, BUC-07, BAS-04 |
| [GOV-04 – Auskunft, Berichtigung, Widerruf und Löschung bearbeiten](https://github.com/marcbey/the-step-agentic-workflow/issues/89) | R2 | P1 | 8 | GOV-03, MIT-06 |
| [GOV-05 – Berechtigungen, Verschlüsselung und Missbrauchsschutz prüfen](https://github.com/marcbey/the-step-agentic-workflow/issues/90) | R1 | P0 | 8 | BAS-03, BAS-04, BUC-02 |
| [GOV-06 – Barrierefreiheit, Ladezeit und Browserqualität abnehmen](https://github.com/marcbey/the-step-agentic-workflow/issues/91) | R1 | P0 | 8 | BAS-06, WEB-01, BUC-02, CMS-04 |

## [E12](https://github.com/marcbey/the-step-agentic-workflow/issues/12) – Migration, Betrieb und Abnahme

| Story | Release | Priorität | Punkte | Abhängigkeiten |
|---|---|---|---:|---|
| [REL-01 – Inhalte und Bestandsdaten kontrolliert migrieren](https://github.com/marcbey/the-step-agentic-workflow/issues/92) | R1 | P0 | 8 | BAS-01, BAS-04, GOV-02, GOV-03 |
| [REL-02 – Betriebsüberwachung und Störungsabläufe vorbereiten](https://github.com/marcbey/the-step-agentic-workflow/issues/93) | R1 | P0 | 5 | BAS-04, BUC-04, GOV-03 |
| [REL-03 – Benutzerhandbuch und rollenspezifische Schulung bereitstellen](https://github.com/marcbey/the-step-agentic-workflow/issues/94) | R1 | P0 | 5 | BUC-08, BUC-09 |
| [REL-04 – Releaseabnahme und agentischen Arbeitsablauf festlegen](https://github.com/marcbey/the-step-agentic-workflow/issues/95) | R1 | P0 | 5 | REL-01, REL-02, REL-03, GOV-05, GOV-06 |

## [E13](https://github.com/marcbey/the-step-agentic-workflow/issues/13) – Optionale Erweiterungen

| Story | Release | Priorität | Punkte | Abhängigkeiten |
|---|---|---|---:|---|
| [EXT-01 – Spenden und Fördermöglichkeiten anbieten](https://github.com/marcbey/the-step-agentic-workflow/issues/96) | R4 | P2 | 8 | FIN-01, FIN-05, GOV-02 |
| [EXT-02 – Installierbare Web-App und optionale Push-Mitteilungen prüfen](https://github.com/marcbey/the-step-agentic-workflow/issues/97) | R4 | P2 | 8 | MIT-06, BUC-09, GOV-01 |
| [EXT-03 – Bewertungen mit Moderation und Schutzregeln anbieten](https://github.com/marcbey/the-step-agentic-workflow/issues/98) | R4 | P2 | 5 | BUC-07, GOV-04 |
| [EXT-04 – Englische Sprachversion für öffentliche Kernabläufe anbieten](https://github.com/marcbey/the-step-agentic-workflow/issues/99) | R4 | P2 | 8 | CMS-01, BUC-04 |
| [EXT-05 – WhatsApp als freiwilligen Kontaktweg verlinken](https://github.com/marcbey/the-step-agentic-workflow/issues/100) | R4 | P2 | 3 | WEB-05, GOV-02 |
| [EXT-06 – Mitglieder werben Mitglieder kontrolliert anbieten](https://github.com/marcbey/the-step-agentic-workflow/issues/101) | R4 | P2 | 5 | MIT-02, MIT-05 |
| [EXT-07 – Skateparks in Stuttgart als Übersicht bereitstellen](https://github.com/marcbey/the-step-agentic-workflow/issues/102) | R4 | P2 | 5 | WEB-05, CMS-01 |
| [EXT-08 – Wetterinformationen für Outdoor-Angebote anzeigen](https://github.com/marcbey/the-step-agentic-workflow/issues/103) | R4 | P2 | 5 | ANG-01, BUC-09 |
| [EXT-09 – Anbindung einer externen Vereins-App spezifizieren](https://github.com/marcbey/the-step-agentic-workflow/issues/104) | R4 | P2 | 5 | MIT-06, GOV-04 |

