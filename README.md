# Durchschaut! Dark Patterns erkennen

Ein Lernspiel für den Unterricht in Medien und Informatik. Schülerinnen und Schüler lernen die 20 Dark Patterns kennen, die die Stiftung für Konsumentenschutz auf [da-pa.ch](https://da-pa.ch) beschreibt, dazu fünf «Zeitfresser», die auf Zeit und Aufmerksamkeit zielen. Sie entlarven alle 25 Tricks in erfundenen Apps selbst.

## Inhalt

Das Spiel besteht aus drei Stationen (im Profi-Niveau vier) und einem Sammelalbum:

- **Trickjagd:** Sieben erfundene Apps in zwei Gruppen. «Einkaufen»: Sneaker-Shop, Ticket-Kasse, Essenslieferung. «Apps & Games»: Game-Shop, Foto-App, Social-Media-App, Chat-App. In der Chat-App stecken an einer Stelle, wie in vielen echten Fällen, zwei Tricks zugleich. Einige Elemente sind bewusst keine Dark Patterns, aber trotzdem heikel (Pay to win, Lootboxen). Sie geben eine Erklärung ohne Punktabzug. Wer nicht weiterkommt, kann eine App auflösen. Sie gilt dann nicht als selbst geschafft.
- **Entkommen:** Acht Missionen in zwei Gruppen. «Nein sagen»: Cookies ablehnen, Cookie-Wall, Abo kündigen, Newsletter abmelden. «Etwas haben wollen»: neue Nutzungsbedingungen, Gratis-Download mit gefälschten Download-Knöpfen, Gewinnspiel, nur kurz ein Video schauen (mit Bildschirmzeit-Anzeige).
- **Was tust du?** Zehn Alltagssituationen, in denen eine App austricksen will. Die Lernenden wählen die passende Schutzreaktion und erhalten einen Tipp. Tricks, die noch nicht verstanden sind, kommen zuerst.
- **Zuordnen (nur Profi):** Zehn Alltagsbeispiele dem Trick zuordnen, der am besten passt. Bei Beispielen, die zu mehreren Tricks passen könnten, begründet die Rückmeldung die Zuordnung.
- **Sammelalbum:** Im Reiter «Tricks» alle 25 Tricks in sechs Kategorien zum Nachlesen, die 20 aus da-pa.ch mit Links zu echten Beispielen in der Hall of Shame. Im Reiter «Abzeichen» die Abzeichen für abgeschlossene Stationen und entdeckte Tricks, dazu ein kurzer Hinweis, dass auch «Durchschaut!» mit Punkten und Abzeichen Gestaltung nutzt, die zum Weiterspielen motiviert.

Es gibt zwei Niveaus. **Einstieg** arbeitet mit einfacher Sprache, Tipps und Fehlklicks kosten keine Punkte. **Profi** verwendet Fachbegriffe mit den englischen Originalnamen, gefundene Tricks müssen benannt werden.

Wer alle Stationen geschafft hat, sieht die **Auswertung «Durchgespielt»**: eine Bilanz, eine Urkunde als SVG-Datei und der Impuls «Augen auf im Alltag»: entdeckte Tricks anderen weitererzählen. «Was tust du?» lässt sich beliebig oft wiederholen. In der Lernbilanz steht bei jedem Trick, wo er im Spiel vorkommt.

Unter «Mein Fortschritt» erstellen die Lernenden eine Lernbilanz mit vier Stufen: *verstanden* (richtig benannt oder zugeordnet, mit Angabe des Niveaus), *entdeckt* (begegnet, aber noch nicht geprüft), *noch unsicher* (aufgelöst oder falsch eingeordnet) und *noch nicht begegnet*. Dazu kommen zwei freiwillige Reflexionsfragen: Wo bist du einem dieser Tricks schon begegnet? Worauf wirst du künftig genauer achten? Punkte, Klickzahlen und Zeiten stehen nicht drin. Die Lernenden entscheiden selbst, ob sie die Datei abgeben.

## Datenschutz

- Keine Anmeldung, kein Tracking, keine Cookies.
- Der Fortschritt wird nur im `localStorage` des Browsers gespeichert. Er lässt sich als Datei oder Spielcode exportieren und auf einem anderen Gerät wieder laden.
- Die Schriften (Atkinson Hyperlegible, Gochi Hand) sind in die Seite eingebettet. Es werden keine Daten an externe Schriftanbieter übermittelt.

## Technik

Die ganze Anwendung steckt in einer einzigen Datei, `index.html`, mit HTML, CSS und JavaScript ohne Frameworks und ohne Build-Schritt. Zum Testen genügt es, die Datei im Browser zu öffnen.

```
index.html             Die Anwendung
favicon.svg            Icon für den Browser-Tab
favicon-32.png         Icon für ältere Browser
apple-touch-icon.png   Icon für den Home-Bildschirm auf iPhone und iPad
og-image.png           Vorschaubild für geteilte Links (1200 × 630)
README.md              Diese Datei
LICENSE.md             Lizenzangaben
```

## Veröffentlichen mit Vercel

1. Neues Repository auf GitHub anlegen und alle Dateien dieses Ordners hochladen.
2. Auf [vercel.com](https://vercel.com) «Add New Project» wählen und das Repository importieren.
3. Bei «Framework Preset» die Option «Other» wählen. Build Command und Output Directory leer lassen.
4. «Deploy» klicken. Jede spätere Änderung auf GitHub wird automatisch neu veröffentlicht.

Das Vorschaubild für geteilte Links ist in `index.html` mit der festen Adresse `https://darkpatterns-durchschaut.vercel.app` verknüpft. Ändert sich die Adresse, müssen die Angaben `og:url`, `og:image` und `twitter:image` angepasst werden.

## Inhaltliche Grundlage

Systematik, Kategorien und Begriffe stammen von [da-pa.ch](https://da-pa.ch), einer Plattform der Stiftung für Konsumentenschutz mit Unterstützung der Stiftung Mercator Schweiz. Erklärungen, Beispiele und Spiele sind eigenständig formuliert. Alle Apps, Marken und Preise im Spiel sind erfunden. «Durchschaut!» ist kein Angebot der Stiftung für Konsumentenschutz.

Die sechste Kategorie «Zeitfresser» (Streaks & Verlustdruck, Endlos-Scrollen, Autoplay, Tägliche Belohnungen, Rückhol-Nachrichten) ist eine eigene Ergänzung. Nicht jede dieser Funktionen ist manipulativ. Problematisch wird es, wenn sie die selbstbestimmte Nutzung gezielt erschwert. Sie stützt sich auf die Forschung zu «Attention Capture Patterns»:

Monge Roffarello, A., Lukoff, K. & De Russis, L. (2023). *Defining and Identifying Attention Capture Deceptive Designs in Digital Interfaces*. CHI 2023, ACM. https://doi.org/10.1145/3544548.3580729

Zudem greift sie Tricks auf, die Medienbildungsangebote wie zischtig.ch als Dark Patterns in Apps und Games beschreiben. Bei jedem Zeitfresser zeigt das Spiel, mit welchem da-pa-Trick er verwandt ist. Die Chat-App ist Snapchat nachempfunden.

Auch die Europäische Kommission empfiehlt in ihren Leitlinien zum Schutz Minderjähriger unter dem Digital Services Act (14. Juli 2025), Funktionen wie Streaks, Autoplay oder Push-Benachrichtigungen bei Minderjährigen standardmässig auszuschalten: https://digital-strategy.ec.europa.eu/de/library/commission-publishes-guidelines-protection-minors

## Entstehung

Programmiert wurde die Seite mit KI-Unterstützung, im sogenannten Vibe Coding mit Claude (Anthropic). Konzept, Texte und Beispiele hat die Herausgeberin geprüft und überarbeitet. Sie trägt die inhaltliche Verantwortung.

## Herausgeberin

Sabrina Meier, Dozentin Medien und Informatik, Co-Leiterin Fachstelle Schule und Digitalität, Pädagogische Hochschule Thurgau
Kontakt: [sabrina.meier@phtg.ch](mailto:sabrina.meier@phtg.ch)

## Lizenz

[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.de). Details in `LICENSE.md`.

Die eingebetteten Schriften Atkinson Hyperlegible und Gochi Hand stehen unter der SIL Open Font License 1.1.
