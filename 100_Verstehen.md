# Verstehen

Mit WordPress verwalten Sie Ihre Seiten und Artikel auch ohne tiefergehende HTML- und CSS-Kenntnisse direkt über den Browser. Für WordPress gibt es Tausende kostenlose Vorlagen ([Themes](https://wordpress.org/themes)) sowie mehr als 47’000 [Plugins](https://wordpress.org/plugins/) mit denen Sie WordPress um unterschiedlichste Funktionen erweitern können.



TODO: Stats update



## Bevor Sie beginnen

Da mit WordPress (wie mit jedem Content Management System) der Inhalt getrennt von der Gestaltung in einer Datenbank abgelegt wird, lässt sich das Design und sogar die Struktur einer Website im Nachhinein ändern ohne die Inhalte zu verlieren.

TODO: abc und Bild

![Schematische Darstellung einer statischen Seite / CMS](images/v4.5/statisch-vs-cms.jpg)

Trotzdem ist es sinnvoll, sich bereits vor der Auswahl eines Themes und vor dem Erfassen des Inhalts über die Anforderungen an die zu erstellende Seite Gedanken zu machen und seinen Internet-Auftritt zu planen:

Q>### Welches primäre Ziel möchte ich mit der Webseite erreichen?
Q>
Q>Eine Website muss heute viel mehr können, als nur eine Visitenkarte zu sein.

- Soll sie zu mehr Umsatz im örtlichen (physischen) Ladengeschäft verhelfen)?
- den Absatz via Internet ermöglichen?
- durch Self-Help / Schulung den Kundendienst entlasten?
- Marketingaufgaben wahrnehmen (Positionierung als Experte) (Achtung: Werbung ist zweischneidig. Aufdringliches Verkaufen schadet)

Q>### Welche Zielgruppe(n) spreche ich an?
Q>
Q>Dies nimmt Einfluss auf die Wort- und Bildsprache, die verwendet werden soll und somit auf die Auswahl eines passenden Themes

Q>### Welche Inhalte werden durch welche Personen verwaltet und wie oft ändern sie sich?
Q>
Q> Antworten auf diese Fragen helfen bei der Entscheidung welche Inhalte als Beiträge (Posts) in verschiedenen Kategorien und welche als Seiten erfasst werden sollen. Auch wird damit klar welche Benutzer angelegt werden müssen und welche Benutzerrolle man diesen zuordnen soll.

Q>### Sollen Besucher des Internet-Auftritts kommentieren, "liken" oder sich beteiligen können?
Q>
Q> Damit werden Entscheidungen für die Einstellungen (Diskussion) gelegt und die Suche nach passenden Plugins oder Funktionen in Themes vorbereitet.

Q>### Wie soll die Website strukturiert werden?
Q>
Q> Gibt es verschiedene Bereiche, und werden Inhalte in Kategorien geordnet? Dies hilft ebenfalls bei der Entscheidung, wie Seiten, Beiträge, Kategorien und Menüs optimal eingesetzt werden.

Grundsätzlich stelle ich fest, dass der Planung und Vorbereitung oft zu wenig Beachtung geschenkt wird. Auch Agenturen erleben immer wieder, dass eine Webseite praktisch fertiggestellt werden kann und "nur noch der Inhalt" geliefert werden muss. Oft sind es jedoch "kleine Anpassungen" die im Verlauf des Projekts anfallen, welche die Projektkosten aus dem Ufer laufen lassen oder die Einhaltung der Termine verunmöglichen.

TODO:

Ich biete daher unter [homepage-abc.ch/projektplan](https://homepage-abc.ch/projektplan) einen kostenlosen, ausführlichen Plan mit Checklisten an.

## Wichtige Begriffe

Bevor wir uns der eigentlichen Verwaltung im Backend zuwenden, möchten ich einige Begriffe klären.

### Frontend und Backend

Unter Frontend versteht man denjenigen Teil der Webseite, welche ein gewöhnlicher Besucher der Website zu sehen bekommt, während das Backend, die Verwaltung der Inhalte und Einstellungen erlaubt. Das Backend von WordPress rufen Sie auf indem Sie im Browser die Adresse der Domain um **/wp-admin** ergänzen, also zum Beispiel: **http://your-company.ch/wp-admin**. Zugriff auf die Verwaltungsoberfläche (Backend) erhält man erst mit der Eingabe eines gültigen Benutzernamens (oder seit WordPress 4.5: der E-Mail Adresse) und dem zugehörigen Passwort.

Aus Sicherheitsgründen empfehle ich das Login in das Backend von WordPress zu erweitern:



TODO: Plugin-Empfehlung und Anleitung.



Es gibt eine grosse Anzahl Sicherheits-Plugins. Die meisten sind aber viel zu komplex und oft verwirrend zu bedienen. Wenn man nicht versteht, was man genau konfiguriert besteht die Gefahr Sicherheitslücken zu öffnen statt zu schliessen oder sich selber auszusperren. Statt eines Plugins, empfehle ich daher mit ein wenig Code das WordPress-Login abzuhärten.

Eine Anleitung und verschiedene weitere Tipps finden Sie in der Broschüre "Mit wenig Code viel erreichen"



TODO: Mit wenig Code viel erreichen schreiben und verlinken



Um einem potentiellen Eindringling keinen Anhaltspunkt zu geben, wird bei einem fehlerhaften Loginversuch nicht angezeigt, ob der Benutzername oder das Passwort falsch war. Ausserdem sind die Loginversuche auf fünf innerhalb von fünf Minuten limitiert. Dem Administrator wird ein E-Mail zugestellt, wenn eine verdächtige Anzahl misslungener Loginversuche erkannt wird. Dies wurde bis vor Kurzem durch das Plugin [Limit Login Attempts](https://wordpress.org/plugins/limit-login-attempts/) gelöst. Da dieses Plugin seit einiger Zeit nicht weiterentwickelt wurde, nutzen wir neu [Cerber Limit Login Attempts](https://wordpress.org/plugins/wp-cerber/)

### Adminleiste

Wenn man im Backend eingeloggt ist, sieht man auch im Frontend die Adminleiste, das heisst am oberen Bildschirmrand wird ein grauer Balken angezeigt, über welchen man direkt auf verschiedene Backend-Funktionen zugreifen kann.

![Adminbar im Frontend, sofern man im Backend eingeloggt ist und entsprechende Rechte hat](images/v4.5/adminbar-my-company.png)

![Beiträge und Seiten in der Adminleiste](images/v4.5/adminbar-neu.png)


Die Erstellung von Beiträgen und Seiten kann so direkt aus dem Frontend heraus gestartet werden. Wenn man Fehler auf einer Seite entdeckt, lässt sich die betroffene Seite im Backend zur Bearbeitung öffnen. Immer wieder gab es auch Versuche, es zu ermöglichen Änderungen direkt im Frontend durchzuführen (z. B. [Editus](https://edituswp.com/), [FrontKit](https://beta.frontkit.io/)).

### Beiträge und Seiten

![Beiträge und Seiten im Hauptmenü](images/v4.5/beitraege-seiten.png))

In WordPress gibt es zwei grundlegende Inhaltstypen: Beiträge und Seiten.

{title="Unterschiede zwischen Beiträgen, Seiten und Custom Post Types"}
| Beiträge (Posts) | Seiten (Pages) | Custom Post Types |
|-|-|-|
| Blog (News) Beiträge | Impressum Über uns | Kontaktformular Veranstaltungen Portfolio |
| chronologisch, Kategorien, Schlagworte (Tags), Archivseiten RSS-Feed | hierarchisch, keine Archivseiten, kein RSS Feed | können wie Beiträge oder wie Seiten gestaltet werden, oft mit Themes/Plugins geliefert, selber programmieren |


Während Seiten direkt hierarchisch angeordnet werden können, lassen sich den Beiträgen Kategorien und Schlagworte (Tags) zuordnen. Standardmässig werden bei Beiträgen ein Veröffentlichungsdatum, Informationen zu Kategorien und Schlagworten sowie Angaben zum Autor (oft erst wenn Beiträge verschiedener Autoren veröffentlicht wurden) angezeigt. So wird es dem Besucher leicht gemacht andere Beiträge aus der gleichen Kategorie oder vom gleichen Autor anzuschauen. Für jede Kategorie, jedes Schlagwort, jeden Autor und jeden Monat gibt es automatisch ein Archiv, in welchem alle zugehörigen Beiträge in einer Übersicht dargestellt werden. Beiträge werden für klassische Blog-Artikel verwendet und eignen sich sehr gut für Nachrichten, Notizen oder Statusmeldungen.

![Kategorien, Autor, Datum und Schlagworte (hier nicht vorhanden) werden automatisch verlinkt](images/v4.5/archive-links.png)

Seiten sind für Inhalte gedacht, die nicht regelmässig erweitert werden, sondern eher beständig sind: eine "Über uns"- oder Impressum Seite, Dokumentationen oder auch Rechtliches. Seiten erscheinen nicht im RSS-Feed ([siehe unten](#rss)) eines Internet-Auftritts. Sie sind unabhängig von der zeitbasierten Darstellung und können hierarchisch angeordnet werden indem ihnen eine Elternseite zugeordnet wird. Einer Seite kann ein Template zugewiesen werden (wenn das Theme dies zur Verfügung stellt). Dadurch lassen sich unterschiedliche Seitentypen beispielsweise mit oder ohne Sidebar aus dem Backend auswählen. Welche Templates zur Verfügung stehen, hängt vom aktiven Theme ab. Gewisse Themes bieten zudem erweiterte Möglichkeiten bei der Seitengestaltung an. Seiten kennen keine Kategorien oder Schlagworte.

![Metabox zur Auswahl der übergeordneten Seite und des Templates im Backend](images/v4.5/eltern-templates.png)

![Darstellung der Seitenhierarchie im Backend](images/v4.5/seitenstruktur.png)


### Post Types/Custom Post Types

Neben den klassischen, bereits erwähnten Inhaltstypen Beiträge (posts) und Seiten (pages) können Themes und Plugins weitere PostTypes zur Verfügung stellen. Häufig vorkommende PostTypes sind "Portfolio", "Testimonials", "Events", "Produkte" oder "Formulare".
Custom Post Types erlauben es Inhaltstypen selber zu definieren und dazu passende Eingabefelder zur Verfügung zu stellen.
Normalerweise programmiert dies der Plugin- oder Theme-Entwickler.

Mehr zu Custom Post Types und praktischen Werkzeugen finden Sie im Kapitel [Erweitern](#erweitern)

### Custom Fields
benutzerdefinierte Eingabefelder sind bei Beiträgen und Seiten standardmässig erfassbar. Ausgegeben werden Sie jedoch erst, wenn die entsprechenden Theme-Template-Dateien im Code angepasst werden. Mit einem Plugin, wie [Get Custom Field Values](https://wordpress.org/plugins/get-custom-field-values/) ist es jedoch möglich auch ohne Eingriff in den Code die Custom Fields auszugeben.

![Beispiel der Ausgabe von Custom Fields. Screenshot von http://your-company.ch/beitrag-mit-benutzerdefinierten-feldern/](images/v4.5/customfield-example.png)

![Ansicht des Backend Beitrags-Editor mit der Metabox zur Erstellung des Shortcodes, wie sie das Plugin Get Custom Field Values zur Verfügung stellt](images/v4.5/customfield-backend2.png)

### Kategorien

{float=left}
![Kategorien Metabox](images/v4.5/kategorien-metabox.png)

Kategorien dienen dazu Beiträge zu klassifizieren. Jeder Beitrag kann einer oder mehreren Kategorien zugeordnet werden. Die Kategorien selbst können hierarchisch verschachtelt werden.


### Tags (Schlagworte)

{float=left}
![Schlagworte Metabox](images/v4.5/tags-metabox.png)

Tags sind Schlagworte, welche einem Artikel unabhängig von der Kategorie zugeordnet werden können. Sie stellen ein weiteres Klassifikationsschema zur Verfügung, welches aber keine Verschachtelung erlaubt.


### Taxonomien
Kategorien und Tags sind sogenannte Taxonomien. Zu Post Types können auch eigene Taxonomien erstellt werden. Für ein _Projektportfolio_ könnte es also statt _Kategorien_ _Projekttypen_ geben oder für einen Custom Post Type _Buch_ wären _Autor_, _Verlag_ etc. geeignete Taxonomien. Taxonomien sind überall dort geeignet, wo eine eins zu mehrere (1:n) Beziehung besteht, also beispielsweise: ein Autor kann mehrere Bücher haben. (Und vielleicht sollte ein Buch auch mehrere Autoren haben können. Beides ist grundsätzlich in WordPress kein Problem).
Das _Erscheinungsdatum_ eine Buches hingegen ist vermutlich in einer Taxonomie nicht gut aufgehoben, sondern benötigt lediglich ein Custom Field, ein benutzerdefiniertes Eingabefeld.

Dies zeigt die praktisch unbeschränkten Anpassungsmöglichkeiten von WordPress für individuelle Projekte. Es kann ratsam sein einen erfahrenen WordPress Consultant, eine mit WordPress vertraute Agentur bzw. einen Webentwickler /-designer zu beauftragen, erforderliche Plugins zu installieren und zu konfigurieren sowie ein Theme zu wählen und anzupassen.


### API - Application Programming Interface
Unter API versteht man die Möglichkeit, interne Funktionen durch Befehlsaufrufe zu nutzen. WordPress steckt voller APIs. Nur dank diesen, ist es relativ einfach möglich WordPress Funktionen in Themes oder Plugins zu nutzen. Muss man beispielsweise Berechtigungen prüfen, kann man auf die entsprechenden API-Befehle zugreifen. Möchte man Inhalte einer externen Seite laden, kann man die HTTP-API von WordPress nutzen. Sollen Daten zuverlässig zwischengespeichert werden, gibt es dafür die Transient-API etc. etc.
In WordPress 4.4 wurde die erste Stufe der REST-API eingeführt, welche es möglich macht WordPress Befehle unabhängig vom WordPress Backend aufzurufen. Mit [Calypso](https://developer.wordpress.com/calypso/) präsentiert Automattic ein Mac-, Windows- und Linux-Programm, welches via Rest-API Inhalte von verbundenen WordPress Seiten bearbeiten kann.


![In Calypso lassen sich fast alle Details von WordPress Seiten bearbeiten](images/v4.5/calypso-menues.png)

{#rss}
### RSS-Feed

![RSS - eine Möglichkeit Beiträge oder Diskussionen zu abonnieren...](images/v4.5/rss-feed.png)

RSS (Real Simple Syndication) ist ein Verfahren um Inhalte (Blog-Posts) einfach zu teilen. Mit Hilfe eines RSS-Readers kann der interessierte Besucher der Webseite die Schlagzeilen, Kommentare oder gesamten Inhalte einer bestimmten Seite (z. B. Kategorie) abonnieren. Ebenso ist es möglich die RSS-Feeds (zum Beispiel von gewissen Branchen-News) aus einer fremden Webseite in die eigene zu integrieren (vergl. [Anpassen/Widgets](#anpassen_widgets) und [Schritt für Schritt/Widgets nutzen](#widgets_nutzen).

![... oder in die eigene Webseite einzubinden](images/v4.5/feed-einbinden.png)

### Theme

Themes sind in WordPress sehr mächtig. Ein Theme kann nicht nur das Aussehen einer Webseite ändern, sondern umfangreiche Funktionen, Formatvorlagen und Einstellungsmöglichkeiten zur Verfügung stellen. Obwohl beim Wechsel eines Themes die Inhalte von Seiten und Posts selbstverständlich erhalten bleiben, kann ihre Darstellung erheblich verändert werden. (z. B. andere Schriftarten und Farben).
Nicht nur wie etwas, sondern auch was überhaupt dargestellt wird, kann vom Theme-Entwickler festgelegt werden.
Informationen, wie Veröffentlichungsdatum, Autor, Kategorie werden daher abhängig vom aktiven Theme angezeigt oder nicht.
Archivseiten können je nach Theme oder Theme-Einstellungen Artikelbilder enthalten und Inhalte im Volltext oder nur als Anreissertext darstellen. Bei der Auswahl eines Themes für die eigene Wordpress-Website sollte man sich daher neben den ästhetischen Aspekten auch von den Anforderungen aus dem Abschnitt "[Bevor Sie beginnen](#bevor_sie_beginnen)" leiten lassen. Im Abschnitt [Anpassen/Wie man ein passendes Theme auswählt](#theme-funktionen) gehe ich weiter auf die Auswahlkriterien für ein geeignetes Themes ein.

### Plugin

Mit Plugins kann WordPress um Funktionen erweitert werden, die es von sich aus nicht bietet. Mit über 47’000 Plugins im [Plugin-Verzeichnis](https://wordpress.org/plugins), lässt sich WordPress um fast jede beliebige Funktionalität ergänzen. Ein Plugin kann beispielsweise E-Commerce und Warenkorb-Funktionalität, ein Kontaktformular, Spamfilter für Kommentare, Newsletter-Management, Bilder-Gallerien mit attraktiven Slidern, Integration mit Facebook und vieles, vieles mehr zur Verfügung stellen. Da Plugins von unabhängigen Entwicklern erstellt werden, variert die Qualität in denen sie programmiert sind deutlich. Das [Plugin-Verzeichnis](https://wordpress.org/plugins) bietet eine Bewertungsmöglichkeit an. Dennoch ist das Auswählen eines geeigneten Plugins eine anspruchsvolle Aufgabe. Bei der switchplus-Installation haben wir für Sie bereits sorgfältig ausgewählte Plugins installiert.

### Widget

Widgets sind durch WordPress Themes oder Plugins bereitgestellte Inhalts-Blöcke, die in Widget-Bereichen (je nach Theme unterschiedlich) ausgegeben werden können. So können Inhalte, wie eine Liste der neuesten Artikel oder Kommentare, ein Formular zum Anmelden an einen Newsletter und vieles mehr ausgegeben werden. Widgets können sehr einfach mit Hilfe von Drag and Drop ind die vorhandenen Widget-Areas positioniert und ein- oder ausgeschaltet werden. Die Anzahl und Positionierung von Widget-Bereichen ist abhängig vom ausgewählten Theme. Manche Themes und Plugins bieten eigene Widgets an, die beim Wechseln bzw. Deaktivieren des Themes bzw. Plugins verloren gehen.

### Gravatar

![Der Gravatar ist ein mit der E-Mail Adresse verknüpftes Bild von gravatar.com](images/v4.5/gravatar.png)

Ein Gravatar ist eine Art Profilbild, welches mit einer E-Mail-Adresse verknüpft ist. Es erscheint in Kommentaren oder Artikeln neben dem Namen. WordPress kann einen Gravatar generieren, wenn die E-Mail Adresse bei [gravatar.com](http://de.gravatar.com/) nicht bekannt ist (siehe Bild).

### Multisite

WordPress lässt sich so konfigurieren, dass mit einer Installation, mehrere unabhängige Blogs (bzw. Websites) betrieben werden können.

## Die Benutzerrollen in WordPress

WordPress bietet von sich aus standardmässig fünf verschiedene Benutzerrollen an:

### Abonnent (Subscriber)

Ein Abonnent kann - wenn er eingeloggt ist - ohne Angabe von Namen und E-Mail-Adresse kommentieren. Diese Angaben werden aus seinem Benutzerprofil geladen, welches er auch selber anpassen kann.

### Administrator (Administrator)

Der Administrator ist der Einzige, der alles kann: Themes und Plugins installieren und ändern sowie alle Einstellungen anpassen.

### Redakteur (Editor)

Der Redaktor kann neben seinen eigenen Artikeln auch diejenigen anderer Autoren ändern und publizieren und kann Seiten erstellen und veröffentlichen.

### Autor (Author)

Der Autor kann Artikel erstellen, sie als Entwurf speichern, "Zur Revision vorlegen", oder auch gleich veröffentlichen.

### Mitarbeiter (Contributor)

Der Mitarbeiter kann Artikel erstellen und "Zur Revision vorlegen". Seine Entwürfe müssen von einem Redakteur (oder dem Administrator) freigeschaltet werden, damit sie veröffentlicht werden.

## Technische Informationen

### MySQL

MySQL ist eines der weitesten verbreiteten relationalen Datenbankverwaltungssysteme und gilt als die populärste Open-Source-Datenbank der Welt. WordPress (und viele andere Web-Anwendungen) nutzen sie zur Speicherung der Daten. Im switchplus Benutzerkonto lässt sich die von WordPress zu verwendende Datenbank über den Menüpunkt "MySQL-Datenbanken" anlegen bzw. verwalten.

### phpMyAdmin

phpMyAdmin nennt sich ein populäres, web-basiertes Administrations-Tool für die Verwaltung von MySQL Datenbanken. Im switchplus Benutzerkonto, kann es über den Befehl "Verwalten" beim Bearbeitungs-Icon jeder Datenbank gestartet werden.

### PHP

Die weitverbreitete Script-Sprache PHP führt auf dem Webserver Befehle aus, um beispielsweise eine Verbindung zur Datenbank herzustellen, Nachrichten via E-Mail zu versenden und vielem mehr. WordPress wurde in dieser Programmiersprache geschrieben.

### Open Source

Open Source bedeutet, dass der "Source Code", die Programmierung einer Anwendung "offen", also frei zugänglich ist. Somit lassen sich von jedermann Funktionen ergänzen oder Fehler korrigieren. Normalerweise stehen Open Source Projekte unter einer Lizenz, wie der GPL, zur Verfügung. Diese fordert, dass Änderungen am Programmcode, die veröffentlicht werden, ebenfalls Open Source sein müssen. 

### HTML (Hypertext Markup Language)

Hypertext Markup Language nennt sich die Sprache, in welcher die Struktur von Webseiten geschrieben wird. Diesen Code können Sie für jede beliebige Webseite einsehen, indem Sie im Browser die Funktion "Seitenquelltext anzeigen" (oder so ähnlich, meistens über Rechtsklick erreichbar) aufrufen.

### CSS (Cascading Style Sheets)

Cascading Style Sheets sind Dateien bzw. der Code, welcher den Stil einer Webseite bestimmt. Mittels CSS steuern Sie das Design von HTML-Elementen (Farben, Abstände, Schriftarten, Hintergründe). Mit einem grundlegenden Verständnis von HTML und CSS sind Sie in der Lage wesentliche Anpassungen am Design (Theme) Ihrer Webseite vorzunehmen, selbst wenn das Theme keine Bearbeitung über den Customizer vorsieht.

T>### Tipp
T>Eine kurze Einführung in HTML & CSS finden Sie im Abschnitt [Kurzer Exkurs in HTML und CSS](#exkurshtmlcss)

### Customizer

Seit Version 3.4 (Juni 2012) von WordPress gibt es den Theme Customizer. Damit lassen sich Änderungen am Theme bequem vornehmen und werden sofort in der Vorschau dargestellt. Zuvor nutzten Theme-Entwickler uneinheitliche Wege zur Verwaltung von Theme-Optionen. Wenn ein Theme heute noch Theme-Optionen zur Verfügung stellt, welche nicht in den Customizer integriert sind, ist das meistens kein gutes Zeichen.

### Child Theme

WordPress kennt den speziellen Mechanismus von Child Themes. Child Themes sind Themes, welche die Funktionalität und Einstellungen aus dem zugehörigen Elterntheme übernehmen. Nur Änderungen bzw. Anpassungen werden im Child Theme definiert. Damit lassen sich Änderungen oft risikofrei ausprobieren. Updates oder Verbesserungen am übergeordneten Theme können vorgenommen werden, ohne die eigenen Änderungen zu überschreiben. Weitere Informationen zu Child Themes finden Sie im [Codex](ttp://codex.wordpress.org/Child_Themes) oder in meiner Präsentation auf [Speaker Deck](https://speakerdeck.com/zu).

### Template Hierarchie

Die Template-Hierarchie ist für Theme-Entwickler interessant, und für WordPress Nutzer, die ein Theme anpassen wollen. Wenn Sie gewisse Kenntnisse in HTML und CSS haben und versuchen ein WordPress Theme anzupassen, werden Sie um Unmengen von Frust nur herum kommen, wenn Sie die WordPress Template Hierarchie verstehen. Ansonsten wissen Sie nicht, wieso Ihre Anpassung manchmal wirkt und manchmal nicht ;-)
Je nach Seitentyp (z. B. Startseite, individueller Beitrag, Beitragsliste einer bestimmten Kategorie…), verwendet WordPress ein anderes Template. Änderungen in der entsprechenden Theme-Datei wirken sich daher nur auf die jeweilige Ansicht aus. Mehr Informationen zur Template-Hierarchie finden Sie im [WordPress Codex](https://developer.wordpress.org/themes/basics/template-hierarchy/)

![Template Hierarchie grafisch dargestellt von http://wphierarchy.com/](images/v4.5/template-hierarchie.png)

Plugins, wie [What The File](https://wordpress.org/plugins/what-the-file/) oder [Query Monitor](https://wordpress.org/plugins/query-monitor/) helfen beim Erkunden, welche Templatedatei auf welcher Seite verwendet wird.