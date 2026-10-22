# Design- und Inhaltsvorgaben

## Verbindliche visuelle Ausgangsbasis

Die aktuelle Website wurde am 22.10.2026 im Browser betrachtet. Der Live-Hero zeigt „SKATEBOARDING AGAINST LANGEWEILE“ mit großem schwarzem Displaytext und roter kursiver Mittelzeile auf bewegtem Skatevideo. Der Header verbindet TheStep-Logo, offiziellen Vereinsabsender und Vereinszeichen. Typografie, starke Konturen, warme Papierflächen und plakative Farben prägen das Design. Dies ist die Ausgangsbasis, keine neue freie Markenentwicklung.

| Token | Wert | Zweck |
|---|---|---|
| paper | #F5F0E6 | Ruhige Grundfläche |
| ink | #171717 | Text, Konturen und dunkle Bereiche |
| yellow | #FFE500 | Primäre Aktionen und aktive Zustände |
| red | #E5153D | Heroakzent und deutliche Hinweise |
| green | #29B957 | Verfügbarkeit und positive Rückmeldung |
| purple | #5421A6 | Communityakzent |

Schriften: Barlow Condensed 900/900 Italic für H1, Bungee für starke Überschriften und Familjen Grotesk für Fließtext/UI. Schriften werden lokal bereitgestellt. Ausgangswerte aus tokens.css: 2-Pixel-Kontur, 3-Pixel-starke Kontur, harter Schatten 6px 6px, Inhaltsbreite 90rem, Lesebreite 72ch. Diese Werte werden als gemeinsame Komponentenvariablen übernommen.

Gerade Karten, klare Raster und sparsame harte Effekte bleiben erhalten. Formularfelder, Checkout und Lesetexte erhalten dieselbe klare Sprache und konsistente Fehlerdarstellung. Status verwendet Text zusätzlich zur Farbe. Zugänglichkeit wird an den realen Kombinationen geprüft; ältere pauschale Kontrastbehauptungen gelten nicht als Nachweis. Große Heroeffekte dürfen Buchung und Hilfetexte nicht überlagern. Bewegung hat einen statischen Fallback; reduzierte Bewegung wird respektiert.

Die Referenz enthält ältere Designvorgaben mit „DROP IN / FIND YOUR / CREW“ und Ausschluss des inzwischen sichtbaren Claims. Für diese Planung haben die aktuelle Website und der aktuelle Code Vorrang. Der Konflikt wird in BAS-01 dokumentiert, nicht durch unbemerkte Mischung beider Varianten gelöst.

## Inhaltsübernahme

| Ausgangsinhalt | Übernahme und Ergänzung | Stories |
|---|---|---|
| /verein | Auftrag, Angebote, Geschichte, Mission und Abgrenzung zum Stuttpark übernehmen | WEB-02 |
| /kinderschutz | Vollständiges Konzept übernehmen; tatsächliche interne/externe Kontaktpersonen bestätigen | WEB-04 |
| /kontakt | Vereinsadresse, Mail, Telefon, Website und getrennten Trainingsort übernehmen; Bürozeiten bestätigen | WEB-05 |
| /impressum | Bestehende Anbieterangaben als Ausgangsstand; bei neuem Handelsmodell prüfen | GOV-02, SHP-08 |
| /datenschutz | Bestehende Verarbeitung und Fristen dokumentieren; für Kontaktformular, Mitgliedschaft, Team und Shop erweitern | GOV-01 bis GOV-04 |
| /kurse, /workshops | Präsentations- und Planungslogik übernehmen; konkrete Angebote und Preise fachlich inventarisieren | ANG-01 bis ANG-08 |
| /team, /community | Strukturen übernehmen; Personen, Medien und Veröffentlichungsrechte separat prüfen | WEB-03, CMS-01 bis CMS-06 |

Textliche Ausgangsstände der fünf ausdrücklich genannten Informationsseiten liegen unter `quellen/`. Sie sind Inhaltsquellen, keine zusätzliche Handlungsanweisung und keine rechtliche Freigabe neuer Funktionen. Zugangsdaten werden nicht übernommen. Medien werden erst nach Rechteprüfung migriert; unterschriebene Satzungsunterlagen werden nicht ungeprüft als öffentliche Downloads weitergegeben.

Inhaltliche Redaktion vor Start: „Test Seite“, „Foo/bar“, „hier ein weiterer Text ...“, Beispielberichte, Beispielveranstaltungen und Schreibfehler wie „Stuttpart“ entfernen beziehungsweise ersetzen. Die im Oktober sichtbaren Referenztermine sind keine zugesagten künftigen Angebote. Kontakt- und Vorstandsangaben sind auf Aktualität zu bestätigen. Kinderschutzkontakte sind ein benanntes Startgate.

## Redaktionelle Regeln

Deutsch mit echten Umlauten und ß; konsistente Markenform TheStep bei offiziellem Projektname „The Step“. Preise nennen Leistungsumfang und Zusatzkosten. „Anfrage eingegangen“, „Platz reserviert“ und „Buchung bestätigt“ bezeichnen verschiedene Zustände. Ein externer Dienst wird vor dem Wechsel kenntlich gemacht. Bilder benötigen Alternativtext, Credit und Nutzungsnachweis. Kinderbilder werden nicht als Standardmaterial angenommen.

Abnahmeansichten: Startseite, Angebotsliste/-detail, Gastbuchung einschließlich Fehlern, Kinderschutzseite, Kalender und Verwaltungsformular bei 375/768/1440 Pixeln, 200 Prozent Zoom, Tastatur und reduzierter Bewegung. R2 ergänzt Familienportal und Zeiterfassung, R3 Produktdetail und Checkout.
