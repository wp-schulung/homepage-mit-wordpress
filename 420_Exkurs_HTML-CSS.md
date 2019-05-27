{#exkurshtmlcss}
# Kurzer Exkurs in HTML und CSS

## Das Web ist nicht aus Papier
Webseiten funktionieren anders als Dokumente, die auf Papier ausgeliefert werden. Obwohl das offensichtlich ist, sind sich manche der Konsequenzen nicht bewusst.

Wenn Sie ein Dokument erstellen, welches ausgedruckt werden soll, oder am Bildschirm als Word oder PDF-Datei betrachtet wird, so bestimmen Sie das Aussehen, die Grösse des Papiers, die Schriftarten, Farben und Anordnung der Elemente.

Bei Webseiten ist das grundsätzlich anders. Sie definieren zwar den Inhalt, aber der Empfänger bestimmt, wie es dargestellt wird. Das mag Sie verwundern und in der Praxis ist es auch nicht ganz so drastisch, aber tatsächlich kontrollieren Sie wesentlich weniger, was Ihre Webseite betrifft, als Sie vielleicht gerne würden.

### Was wir nicht wissen können
- Wir wissen nicht welchen Browser oder «User Agent» der Besucher benutzt.
- Wir kennen die Grösse des Bildschirms, oder wie gross das Browserfenster eingestellt ist nicht.
- Wir haben keine Ahnung, mit welcher Verbindungsgeschwindigkeit unser Besucher verbunden ist, oder wie zuverlässig seine Internetverbindung ist.
- Wir kennen weder die Leistungsklasse seines Computers, noch wissen wir, welches Betriebssystem er besitzt oder welche Schriften auf seinem Computer installiert sind.
- Wir wissen ausserdem nicht, wo sich der User befindet, wie er denkt, welche Sprachen er versteht, und wie gut er oder sie sich mit Computern auskennt.

Aus all diesen Gründen haben wir nur teilweise die Kontrolle darüber, wie die Seite beim Empfänger dargestellt wird. Der Browser, also das Programm, welches die Webseite für den Benutzer darstellt, liest den Quellcode der Seite ein und interpretiert (rendert) die Seite.

### Aufbau einer Webseite
Wenn Sie also eine Webseite erstellen, kreieren Sie nicht eine fix definierte Seite, sondern lediglich eine Struktur und gewisse Formatierungsanweisungen, die aber abhängig vom verwendeten «User Agent» und den Einstellungen beim Benutzer deutlich unterschiedlich «gerendert» werden können. 

#### Verschiedene Sprachen
Eine einzelne Webseite besteht aus Code-Anweisungen (Quelltext) in mehreren Sprachen:

![Code-Sprachen einer Webseite](images/v4.5/sprachen-html-css-js.jpg)

##### HTML
Die Struktur einer Seite wird in der Hypertext Markup Language (HTML) geschrieben. Diese «Auszeichnungssprache» dient dem Ordnen des Inhalts. Darin definieren Sie Layoutbereiche, Überschriften, Absätze, Listen, Links, Bilder und so weiter. Erst mit Hilfe von Cascading Stylesheets (CSS) geben Sie Gestaltungsanweisungen für die HTML-Elemente.

##### CSS
Mit CSS definieren Sie Farben, Abstände, Ränder, Schriftarten, also das Styling und Design der Webseite. Ausserdem können mit CSS die Anordung der Layoutbereiche bestimmen, was schon ziemlich knifflig sein kann. 

##### JavaScript
Schliesslich können Sie mit Hilfe von JavaScript das Verhalten von Elementen (beispielsweise beim Darüberfahren mit der Maus) beim Klicken, beim Senden eines Formulars etc. beeinflussen. Effekte wie das Vergrössern eines Bildes beim Klicken und Abdunkeln des Hintergrunds (Lightbox-Effekt) oder manche Dropdown-Effekte bei Menüs werden mit Hilfe von JavaScript ausgeführt. Auch das Überprüfen von Formularinhalten und die Meldung dass die E Mail-Adresse ungültig sei, geschieht mit Hilfe von JavaScript.

Ale diese drei Sprachen werden von Ihrem Browser ausgeführt und sind darum auf Ihrem PC unverschlüsselt sichtbar. Mit Hilfe von eingebauten Browser-Funktionen können Sie sowohl den Code sehen wie auch Änderungen vornehmen, die auf der gerade aktiven Seite sichtbar werden. Dauerhaft speichern lassen sich solche Manipulationen nur durch Anpassung der betroffenen Dateien auf dem Server. Bei WordPress kann es ziemlich tricky sein, diese heraus zu finden, da die im Browser dargestellte Seite auf dem Server aus verschiedenen Dateien zusammengesetzt wird.

#### Aufbau der HTML-Datei und HTML-Grundgerüst
Jede HTML-Datei besteht aus der Dokumenttyp-Definition, dem HTML-Root-Element sowie einem Head und einem Body.

Die Dokumenttyp-Definition (Doctype declaration) muss in der ersten Zeile des HTML-Dokuments stehen und erklärt dem Browser, welcher Dokumenttyp nun folgt und um welche HTML-Version es sich dabei handelt. Während die früheren HTML Versionen zum Teil eine mehrzeilige und komplexe Dokumenttyp-Definition erforderten, genügt beim aktuellen HTML 5 ein einfaches:

    <!DOCTYPE HTML>

Anschliessend folgt das HTML-Stammelement **<html>**, in welches die beiden Blöcke **<head>** und **<body>** eingefügt werden. 
Beim **<head>** handelt es sich um eine Art Vorspann für die Webseite, welcher nicht im Textfenster des Browsers erscheint. Die Informationen darin werden jedoch von Browsern oder Suchmaschinen ausgewertet. Der Inhalt des **<title>**-Tags erscheint in der Titelleiste des Browsers und wird im Browser-Verlauf, bei den Bookmarks (Favoriten) und auf der Suchresultate-Seite von Suchmaschinen angezeigt. Ebenfalls von Suchmaschinen ausgewertet werden Informationen des **<meta>**-Tags.

Im **<body>**-Bereich steht der eigentliche Inhalt der Webseite, jeweils innerhalb von Tags.

Die meisten Tags bestehen aus einem öffnenden und einem schliessenden Tag, z. Bsp. **<h1></h1>**. Der eigentlich Inhalt steht dazwischen: <h1>Hallo Welt</h1>

Solche HTML-Elemente, bestehend in der Regel aus einem Anfangs- und einem Ende-Tag und dem eigentlichen Inhalt. Sie können (oder müssen) zusätzlich Attribute haben. Attribute sind im öffnenden Tag zusätzlich erfasste Werte, die verschiedene Eigenschaften des Tags auszeichnen. Bei Bildern ist das beispielsweise der Pfad zur Bild-Datei, der Alternativ-Text, der angezeigt wird, wenn die Bild-Datei nicht geladen werden kann oder die Höhe und Breite des Bildes, welche dem Browser hilft, die Seite schon korrekt aufzubauen, auch wenn die Bilddatei noch nicht fertig geladen wurde.

Zusätzlich können Attribute verwendet werden um einem HTML-Element eine ID (die pro Seite nur einmal vorkommen darf) oder eine Klasse (die mehrmals vorkommen kann) zuzuordnen. Diese sind beim Stylen mit CSS wichtig weil man somit Stilanweisungen ganz gezielt vergeben kann.

![Aufbau einer HTML-Datei](images/v4.5/Slide-HTML-Datei.jpg)

![Aufbau HTML-Element. Im Beispiel ist der Inhalt des a-Elements ein Bild, also ein weiteres HTML Element. Es könnte auch reiner Text sein.](images/v4.5/html-element.png)

Bei WordPress wird der Grossteil der HTML-Struktur durch das verwendete Theme vorgegeben und viele Elemente (zum Beispiel die Navigation) werden dynamisch generiert. Wenn Sie hier also etwas ändern möchten, müssen Sie wissen in welcher Theme-Datei der Code steht oder durch welche Funktion er generiert wird.

##### HTML-Elemente und ihre Verwendung

![Die wichtigsten HTML-Elemente und Attribute 1/2](images/v4.5/elemente-und-attribute.png)

![Die wichtigsten HTML-Elemente und Attribute 2/2](images/v4.5/elemente-und-attribute2.png)

Eine Liste der HTML5-Elemente gibt es im [Mozilla Developer Network](https://developer.mozilla.org/de/docs/Web/HTML/HTML5/HTML5_element_list)

Welche Elemente und Attribute von welchen Browsern unterstützt werden, wird übersichtlich dargestellt von [http://caniuse.com/](http://caniuse.com/)

##### Pfadangaben im HTML Code
Die Pfadangaben bei internen Links oder zu Bildern und Stylesheets können absolut oder relativ angegeben werden. Absolut bedeutet: die ganze URL, inkl. Protokoll wird eingetragen, also die gleiche Adresse, die man auch im Browser eingeben würde um die Seite (oder das Bild) aufzurufen. Relativ bedeutet: man lässt den Anfang des Pfades weg und gibt nur den Weg von der aktuellen Position zur Datei an. Bei einem Bild, welches im gleichen Ordner liegt, wie die HTML-Datei heisst das, nur den Dateinamen, z. B.

    <img src="Einstieg-n2.png">

Würde das Bild in einem Ordner «images» liegen, müsste der Pfad entsprechend angepasst werden:

    <img src="images/Einstieg-n2.png">

Wichtig ist darauf zu achten, dass die Pfadangabe ohne «/» beginnt, sonst wird ein sogenannter Root-relativer Pfad verwendet. Das «/» entspräche somit dem «/» nach .ch.
Um bei der relativen Pfadangabe in der Ordnerstruktur eins nach oben zu springen verwendet man zwei Punkte:

    src="../Ordner/Dateiname">

In WordPress werden die meisten Pfadangaben generiert. WordPress kennt verschiedene Befehle, die in Themes-Dateien genutzt werden können um die Pfadangabe, zum Beispiel zum Themeverzeichnis, zu erstellen. Genaue Angaben dazu macht der [Codex](http://codex.wordpress.org/Stepping_Into_Templates)

#### CSS Crash-Kurs
Mit HTML können wir die Struktur der einzelnen HTML-Seiten und die Verlinkung zueinander, also eine Navigation erstellen und so unseren Internet-Auftritt (Website) erstellen. Damit die Schriftarten, Farben, Grössen so aussehen, wie wir das gerne hätten, müssen wir der HTML-Datei noch Style-Anweisungen mitgeben. Ansonsten wird unsere Seite einfach mit den Standardstylen designt.
Style-Anweisungen können an drei Orten eingegeben werden

1. in einer externen CSS-Datei, welche im **<head>** verlinkt wird.
Dies ist die übliche und empfohlene Methode.
Vorteil: Stile können an einem Ort definiert werden und gelten für alle Seiten des Internet-Auftritts (welche dieses Stylesheet verwenden). In WordPress ist die Haupt-CSS Datei mit Ordner des Themes und heisst styles.css. Diese wird automatisch aufgerufen.

2. durch CSS-Anweisungen direkt im <head>

3.  als style-Attribut direkt bei einem HTML-Element
Vorteil: Sie können ein einzelnes Wort oder einen Absatz unabhängig vom CSS gestalten. In WordPress können Sie durch Anweisungen im HTML-Code des Editors so gewisse Anpassungen vornehmen.
Nachteil: Formatanweisungen im externen Stylesheet werden überschrieben

#### Aufbau einer CSS-Anweisung
Eine CSS-Anweisung besteht immer aus einem **Selektor** und einem oder mehrerer Paare aus **Eigenschaft** und **Wert**. Der Selektor bestimmt, auf welches oder welche HTML-Elemente die nachfolgenden Eigenschaften angewendet werden sollen.

Das folgende Beispiel zeigt eine CSS-Anweisung, die dafür sorgt, dass alle Überschriften 1. Ranges eine rote Schriftfarbe erhalten.

![CSS-Anweisung, die Überschriften (h1) rot einfärbt.](images/v4.5/css-example.png)

Selektoren beziehen sich auf ein bestimmtes HTML-Element, auf HTML-Elemente mit einer bestimmten ID oder Klasse (dargestellt durch # für eine ID und . für eine Klasse) oder auch eine Pseudoklasse, wie zum Beispiel a:hover, was sich auf einen Link bezieht solange man mit der Maus darüber fährt.

Ein gewöhnlicher Element-Selektor bezieht sich auf ein einzelnes Element oder auf eine durch Kommata getrennte Gruppe von Elementen.

Durch Leerschläge getrennte Elemente kennzeichnen einen kontextsensitiven Selektor. Damit kann man beispielsweise nur Listenelement innerhalb der Navigation ansprechen. 

Der Selektor

    #masthead h1.site-title

zielt beispielsweise gezielt auf Überschriften 1. Ranges mit der Klasse "site-title", die sich innerhalb eines HTML-Elements mit der ID masthead befinden.

Für weitere Informationen zu HTML und CSS empfehle ich: [Little Boxes](http://little-boxes.de/) von [Peter Müller](http://pmueller.de/) und die verschiedenen Online-Referenzen.
Eine sehr gutes kostenloses Tutorial auf Englisch ist: [MarkSheet](http://marksheet.io/).

