# Durchschaut! Dark Patterns erkennen

Ein Lernspiel für den Unterricht in Medien und Informatik. Schülerinnen und Schüler lernen die 20 Dark Patterns kennen, die die Stiftung für Konsumentenschutz auf [da-pa.ch](https://da-pa.ch) beschreibt, und entlarven sie in erfundenen Apps selbst.

## Inhalt

Das Spiel besteht aus drei Stationen und einem Sammelalbum:

- **Trickjagd:** Sechs erfundene Apps (Sneaker-Shop, Game-Shop, Foto-App, Ticket-Kasse, Essenslieferung, Social-Media-App) mit je vier verdächtigen Stellen. In der Social-Media-App stecken mehrere Tricks in einer Stelle, wie in vielen echten Fällen.
- **Entkommen:** Vier Missionen: Cookies ablehnen, Cookie-Wall, Abo kündigen, neue Nutzungsbedingungen. Ein Klickzähler macht sichtbar, wie viel Aufwand das Ablehnen kostet.
- **Zuordnen:** Zehn Alltagsbeispiele den richtigen Tricks zuordnen.
- **Sammelalbum:** Im Reiter «Tricks» alle 20 Tricks in fünf Kategorien zum Nachlesen, mit Links zu echten Beispielen in der Hall of Shame von da-pa.ch. Im Reiter «Abzeichen» die Abzeichen für abgeschlossene Stationen und entdeckte Tricks.

Es gibt zwei Niveaus. **Einstieg** arbeitet mit einfacher Sprache, Tipps und Fehlklicks kosten keine Punkte. **Profi** verwendet Fachbegriffe mit den englischen Originalnamen, gefundene Tricks müssen benannt werden.

Unter «Mein Fortschritt» erstellen die Lernenden eine Lernbilanz: welche Tricks sie erkennen, wo sie unsicher sind und welchen sie noch nicht begegnet sind, dazu zwei freiwillige Reflexionsfragen. Punkte, Klickzahlen und Zeiten stehen nicht drin. Die Lernenden entscheiden selbst, ob sie die Datei abgeben.

## Datenschutz

- Keine Anmeldung, kein Tracking, keine Cookies.
- Der Fortschritt wird nur im `localStorage` des Browsers gespeichert. Er lässt sich als Datei oder Spielcode exportieren und auf einem anderen Gerät wieder laden.
- Die Schriften (Atkinson Hyperlegible, Gochi Hand) werden von Google Fonts geladen. Dabei wird die IP-Adresse an Google übermittelt.

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

## Entstehung

Programmiert wurde die Seite mit KI-Unterstützung, im sogenannten Vibe Coding mit Claude (Anthropic). Konzept, Texte und Beispiele hat die Herausgeberin geprüft und überarbeitet. Sie trägt die inhaltliche Verantwortung.

## Herausgeberin

Sabrina Meier, Dozentin Medien und Informatik, Co-Leiterin Fachstelle Schule und Digitalität, Pädagogische Hochschule Thurgau
Kontakt: [sabrina.meier@phtg.ch](mailto:sabrina.meier@phtg.ch)

## Lizenz

[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.de). Details in `LICENSE.md`.
