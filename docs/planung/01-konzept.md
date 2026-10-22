# The Step – Produktkonzept

Stand: 22. Oktober 2026. Status: ausgearbeitete Planung zur fachlichen Prüfung; keine Behauptung einer bereits implementierten oder rechtlich freigegebenen Anwendung.

## Auftrag und Erfolg

TheStep erhält einen zusammenhängenden digitalen Auftritt für den Stuttgarter Skateboard e.V.: informieren, passende Angebote finden, anmelden, im Verein mitmachen und den laufenden Betrieb organisieren. Grundlage sind fünf Anforderungsfotos, die aktuelle Website und die technischen Rahmenbedingungen aus „TheStep Verein“. Gewünscht ist die vollständige Planung im Repository und GitHub-Projekt; eine Umsetzung der Produktsoftware oder Änderung am bestehenden Betrieb ist nicht Teil dieses Auftrags.

Erfolg bedeutet: Jeder Inhalt der Fotos ist einer überprüfbaren Story zugeordnet. Ein erster nutzbarer Release bietet Website und verlässlichen Buchungsbetrieb; alle weiteren gewünschten Bereiche sind in abhängigen Releases ausgearbeitet. Jede Story hat konkrete AKs, Priorität, fachliche Abhängigkeiten, Prüffälle und eine Aufwandshypothese. Unbekannte Preise, Fristen und Geschäftsmodelle bleiben als benannte Entscheidungen sichtbar.

## Zielgruppen und Aufgaben

| Zielgruppe | Wichtigste Aufgaben |
|---|---|
| Kinder, Jugendliche, erwachsene Einsteiger | Passendes Level finden, Termine verstehen, sicher teilnehmen |
| Eltern und Sorgeberechtigte | Sicherheit prüfen, Kind anmelden, Ausrüstung und Kosten verstehen, Buchung ändern |
| Mitglieder und Förderer | Antrag, Beiträge, Änderungen, Vorteile, Belege und Dokumente |
| Coaches und Mitarbeitende | Einsätze, notwendige Teilnehmerdaten, Check-in, Stunden, Abwesenheiten und Material |
| Büro, Redaktion, Kursplanung und Kasse | Inhalte freigeben, Termine planen, Buchungen bearbeiten, Nachrichten und Abrechnung |
| Schulen, Gruppen, Sponsoren und Presse | Zusammenarbeit anfragen, Informationen und freigegebene Materialien erhalten |
| Shopkunden und Shopteam | Produkte, Mitgliederpreise, sichere Bestellung und nachvollziehbare Abwicklung |

Ein Zugang kann mehrere Aufgaben besitzen. Öffentliche Teamdarstellung, Verwaltungsrolle, Coachzuständigkeit und Vereinsmitgliedschaft bleiben unabhängige Eigenschaften. Kinder benötigen für eine Buchung kein eigenes Login.

## Informationsarchitektur

Die sieben Hauptbereiche aus IMG_1143 werden übernommen. Die Navigation wächst mit tatsächlich freigegebenen Funktionen; noch leere Shop- und Portalziele werden nicht als fertige Angebote präsentiert.

| Bereich | Inhalte und zentrale Aktion |
|---|---|
| Startseite | Prägender Hero, nächstes Training, Camps, aktuelle Events/News, „Skateangebot finden“ |
| Skateangebote | Kurse, Schnupperkurse, Camps, Workshops, Geburtstage und Gruppen/Schul-AGs; filtern, buchen oder anfragen |
| Events | Landesmeisterschaften, Contests, Jam Sessions, School’s Out, Ferienprogramme, Kalender und Anmeldung |
| Verein | Auftrag, Geschichte, Werte, Team/Vorstand, Mitgliedschaft, Beiträge, Vorteile, Satzung, Ehrenamt/Jobs, Kinderschutz |
| Shop | Kleidung, Skateboards, Decks, Rollen, Zubehör, Merch, Vereinskollektion und Gutscheine |
| News | Ankündigungen, Berichte, Bilder, Videos, Presse und optionaler Social-Einstieg |
| Mein TheStep | Eigene/freigegebene Familienbuchungen, Mitgliederdaten, Belege, Dokumente; rollenabhängig Mitarbeiterwerkzeuge |

Kontakt, Standorte/Anfahrt, Hilfe/FAQ, Sicherheit/Ausrüstung, Sponsoren, Impressum, Datenschutz, Einstellungen und Erklärung zur Barrierefreiheit bleiben über passende Kontexte und den Footer erreichbar. Kinderschutz erhält zusätzlich einen direkten sichtbaren Einstieg. Suche durchsucht ausschließlich öffentliche Inhalte.

## Zentrale Abläufe

**Gastbuchung:** Angebot und Termine prüfen → Preisgruppe/Ausrüstung wählen → notwendige Teilnehmer- und Elternangaben erfassen → Preis und Datenschutzhinweis prüfen → zeitlich begrenzt reservieren → E-Mail-Link bestätigen → verbindliche Bestätigung erhalten. Der Platz ist maximal 60 Minuten reserviert, spätestens bis Angebotsbeginn. Die Kapazität wird in der Datenbank entschieden; eine veraltete Browseranzeige kann keine Überbuchung erlauben. Zahlung erfolgt im ersten Release vor Ort.

**Volles Angebot:** bestätigter Wartelisteneintrag → fairer Rang → befristetes Nachrückangebot → Annahme über denselben Kapazitätsprozess. Vorgeschlagen sind FIFO und 24 Stunden Annahmefrist, maximal bis Buchungsschluss; vor Umsetzung wird diese Regel fachlich bestätigt.

**Regelmäßiger Kurs:** Ein explizites Block-/Einzelterminmodell schließt die Referenzlücke. Blockbuchung reserviert alle erforderlichen Termine gemeinsam. Keine automatische Teilzusage bei einer vollen Woche. Serienänderungen benötigen eine Vorschau ihrer Folgen für bestehende Anmeldungen.

**Geburtstag/Gruppe:** Anfrage → Prüfung von Halle, Zeit und Betreuung → befristetes Angebot → Annahme und planerische Freigabe → verbindliche Veranstaltung. Ein automatischer Eingangstext verspricht noch keinen Termin. Schul-AGs und Firmenangebote folgen demselben Anfrageprinzip mit eigenen notwendigen Feldern.

**Mitgliedschaft:** Bedingungen lesen → Antrag mit zutreffender Vertretung → fachliche Aufnahmeentscheidung → Status/Mitgliedsnummer → zentrale Vorteilsprüfung und Beitragslauf. Ein Antrag ist keine aktive Mitgliedschaft. Änderungen und Kündigungen erhalten bestätigte Wirksamkeitsdaten.

**Kursbetrieb:** Kursplanung besetzt Termine → Coach sieht die eigenen berechtigten Termine → notwendige Teilnehmerdaten und tagesbezogener Check-in → dokumentierte Änderungen. Zuordnungsentzug wirkt sofort. Stunden werden unabhängig erfasst, eingereicht und geprüft; Abrechnung ist kein automatischer Zahlungsvorgang.

**Shop:** Produkt/Variante → serverseitiger Preis einschließlich Mitgliedervorteil → bestandssicherer Warenkorb → gehosteter Checkout → verifizierter Zahlungsstatus → Bestellung/Beleg → Versand oder Abholung → geregelte Rückgabe/Erstattung. Gutscheinrestwerte sind atomar; Rückkehr vom Zahlungsanbieter gilt allein nicht als Zahlungsnachweis.

## Architekturansatz und Alternativen

Empfohlen wird ein zusammenhängender Rails-Monolith mit klar getrennten fachlichen Bereichen und selektiver geprüfter Wiederverwendung aus „TheStep Verein“. Gemeinsame Identität, Inhalte und Buchung vermeiden doppelte Stammdatenpflege. Hotwire ergänzt serverseitige Ansichten. Eine API wird erst für eine konkret beschlossene Integration gebaut.

Ein vollständiger Fork kann schneller starten, übernimmt aber historische Prototypgrenzen, veraltete Texte und migrationsbezogene Altlasten. Ein vollständiger Neubau erlaubt einen sauberen Start, verliert jedoch bereits gelöste Buchungs-, Berechtigungs- und Medienfälle. BAS-01 entscheidet anhand des realen Bestands, welche Komponenten übernommen werden. Das Grunddesign und die verifizierten technischen Versionen sind unabhängig davon gesetzt.

Für den Shop bleibt eine echte Wahl zwischen Rails-Integration und gehostetem Handel offen. Mitgliedschaft und Vorteilsberechtigung bleiben auch bei externem Shop fachlich kontrolliert. Der bestehende Server und das bestehende Repository werden im Planungsauftrag nicht verändert.

## Umfang und Ausbaustufen

- R0: Referenzabgleich, reproduzierbare Basis, Berechtigungen, Design und isoliertes Staging.
- R1: Öffentliche Website, Redaktion, Angebote einschließlich regelmäßiger Anmeldung, sichere Buchung, Warteliste, Events, Teilnehmerbetrieb, Vor-Ort-Zahlungsvermerk und Releasegates.
- R2: Mitgliedschaft, Familienportal, Beiträge/Rechnungen, Teamorganisation und freiwilliger Newsletter.
- R3: Shop, Zahlungsanbindung, Bestellungen und digitale Gutscheine; Online-Zahlung für Kurse benötigt eigene fachliche Aktivierung.
- R4: Ausgearbeitete optionale Extras einschließlich Social Feed, Spenden, PWA/Push, Bewertungen, Englisch, WhatsApp, Empfehlungen, Skateparks, Wetter und konkrete Vereins-App-Anbindung.

Kein Bereich aus den Fotos wird stillschweigend gestrichen. Optionale Vorschläge aus den Fotos sind priorisierbare Stories und keine bereits genehmigten neuen Datenverarbeitungen. Vollständige Planung bedeutet hier einen vollständigen Weg zum Ziel einschließlich der Entscheidungen, die nur der Verein treffen kann.
