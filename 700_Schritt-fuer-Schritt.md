-# Teil 2: Anwenden und Üben {#teil-2}

# Schritt für Schritt

## Grundeinstellungen

### Einstellungen vornehmen

Nehmen Sie die für Sie passenden Einstellungen vor.

-   Passen Sie die administrative E-Mail-Adresse an. (Einstellungen/Allgemein/E-Mail Adresse)
-   Titel der Webseite und Untertitel (via Einstellungen oder Design/Anpassen —> Customizer)
-   Stimmt die Zeitzone und das Datums- und Zeitformat?
-   Sollen sich Benutzer registrieren dürfen (Einstellungen/Allgemein - oder zum Kommentieren müssen, vergl. Einstellungen/Diskussion)?
-   Welche Einstellungen sind optimal um Kommentare zu erlauben aber Spam möglichst auszuschliessen?
-   Wie sollen die Permalinks (dauerhafte URLs für Beiträge und Seiten) aussehen?
-   Was soll die Startseite sein?
-   Passen die Bildgrössen zum Theme? (das muss sonst später angepasst werden: Plugin [Regenerate Thumbnails](https://wordpress.org/plugins/regenerate-thumbnails/) u. ä.)

### Zusatzaufgaben:

-   Testen Sie das Press This Bookmarklet (Werkzeuge / Verfügbare Werkzeuge) (vergl. [Wie kann ich „Press This“ von WordPress nutzen?](https://switchie.ch/wie-kann-ich-press-this-von-wordpress-nutzen/)

## Bedienen - WordPress als Blog nutzen

### Beiträge erfassen

Erfassen Sie etwa 6-7 kurze Beiträge. Je nach Theme stehen Ihnen dazu unterschiedliche Formatvorlagen/Layouts zur Verfügung. 

Achten Sie darauf, dass Sie Beiträge mit unterschiedlichen Formatvorlagen erstellen. (Standard, Kurzmitteilung, Bild, Link, Zitat, Statusmitteilung)

### Beitrag (Standard) formatieren

Bauen Sie den Beitrag "[Ein weiterer Beitrag mit Standard-Formatvorlage](http://your-company.ch/standard-bsp-formatiert/)" nach.

### Kategorien und/oder Schlagworte nutzen

Erstellen Sie die Kategorien "WordPress” und “Formatvorlage” auf zwei Arten: Einmal aus "Beitrag bearbeiten" und einmal aus "Beiträge/Kategorien". Ordnen Sie die erstellten Beiträge jeweils einer oder mehreren Kategorien zu und versehen Sie die Beiträge ebenfalls mit Schlagworten.

Schauen Sie sich an, wie die Kategorien- und Schlagwortseiten aussehen indem Sie bei den Meta-Informationen eines Beitrags auf den entsprechenden Link klicken.

#### Zusatzaufgaben:

-   Kontrollieren Sie die Einstellungen unter "Diskussion" und stellen Sie sicher, dass Kommentare erlaubt sind und sowohl Pingbacks als auch Trackbacks aktiviert sind.

- Kommentieren Sie einen Beitrag auf dem Blog eines Mitschülers.
- Erstellen Sie einen neuen Beitrag (zum Beispiel mit dem Bookmarklet "Press This") in welchem Sie einen Link zu einem beliebigen Beitrag auf dem Blog eines Mitschülers setzen.
- Geben Sie erhaltene Kommentare frei. Fordern Sie Ihre Mitschüler auf noch einmal zu kommentieren und antworten Sie auf den Kommentar.


## Bedienen - WordPress als CMS nutzen

### Seiten erfassen

Erstellen Sie eine **Über uns**, eine **Impressum** und eine **Kontakt**-Seite. (Auf der Kontaktseite fügen wir später das Kontaktformular ein. Im Moment genügt es, wenn Sie den Titel und die Adresse erfassen)

{#widgets_nutzen}
### Widgets nutzen

Nutzen Sie ein paar der verfügbaren Widgets (Z. B. Kategorien, Letzte Beiträge, Schlagwörter-Wolke) Erstellen Sie Inhalt in einem Textwidget und aktivieren Sie es in einer Widget-Area. Binden Sie den RSS Feed (https://www.switchplus.ch/kurs-uebersicht/feed/) mit den nächsten Schulungsterminen von switchplus (oder einen beliebigen anderen Feed) in Ihre Seite ein. Schalten Sie das Text-Widget aus ohne den Inhalt zu verlieren (Inaktive Widgets)

### Menü gestalten

Gestalten Sie ein Menü mit einer Struktur für die einzelnen Seiten und Kategorien und/oder Schlagworten. Weisen Sie dieses Menü dem Primären Menubereich (je nach Theme unterschiedlich benannt) zu.

T>#### Hinweis
T>Menü-Einträge zu Beiträgen können erst gesetzt werden wenn unter _Design/Menüs_ “Ansicht anpassen” die Box “Beiträge” ausgewählt wurde.

### Benutzer erstellen

Erstellen Sie im Backend einen Benutzer mit "Mitarbeiter"-Rechten. Loggen Sie sich aus und als diesen neuen Benutzer wieder ein und erstellen Sie einen Beitrag. Loggen Sie sich wieder aus und als Administrator ein um den Beitrag freizugeben.

T>#### Hinweis
T>Wenn Sie oft verschiedene Rollen testen müssen, empfehle ich das Plugin "[User Switching](http://wordpress.org/plugins/user-switching/)".

## Erweitern

### Kontaktformular erstellen

Installieren Sie das Plugin [Contact Form 7](http://wordpress.org/plugins/contact-form-7/) oder [WPForms Lite](https://wordpress.org/plugins/wpforms-lite/) richten Sie es ein. Fügen Sie den Shortcode auf der Seite **Kontakt** ein. Testen Sie das Formular. (Nutzen Sie dazu möglichst eine E-Mail-Adresse auf die Sie jetzt Zugriff haben)
Alternativen für komplexere Formulare: [Torro Forms](https://wordpress.org/plugins/torro-forms/) [Ninja Forms](http://wordpress.org/plugins/ninja-forms/), [Caldera Forms](https://wordpress.org/plugins/caldera-forms/), [Gravity Forms](http://www.gravityforms.com/) (kostenpflichtig).

### Antispambee installieren

Von Automattic gibt es ein wirksames Antispam-Plugin namens [Akismet](https://akismet.com/). Die Benutzung von Akismet ist für Privatanwender kostenlos, setzt aber eine Registrierung bei wordpress.com voraus. [Antispambee](https://wordpress.org/plugins/antispam-bee/) ist eine deutsche Alternative, welche ohne die, (vorallem in Deutschland) umstrittene Datenhaltung von vollständigen IP-Adressen auf ausländischen Servern, auskommt. 

### Cerber Limit Login Attempts installieren

[Cerber Limit Login Attempts](https://wordpress.org/plugins/wp-cerber/) ist ein Sicherheitsplugin, welches Loginversuche einschränkt und dadurch einen guten Schutz gegen Brute Force Attacken bietet.

### Beliebiges eigenes Plugin installieren

Vorschläge: WooCommerce, Events Manager, TablePress, Lightweight Grid Columns, Simple CSS, GoWorks Styler, Page Builder by SiteOrigin, Soliloquy Lite, JetPack, Easy Digital Downloads, BirchPress, Paid Memberships Pro, Query Monitor, MailPoet Newsletters, Postmatic, User Switching ...

### Plugin aktivieren/deaktivieren, Plugin Dateien löschen

Nachdem Sie verschiedene Plugins installiert und aktiviert haben, deaktivieren Sie nun das eine oder andere Plugin. Löschen Sie anschliessend ebenfalls die Dateien aus dem Backend. Kontrollieren Sie evtl. mit FTP, ob die Dateien aus dem Pluginverzeichnis (/wordpress/wp-content/plugins/) entfernt wurden.

#### Zusatzaufgabe:

Was passiert, wenn Sie den umgekehrten Weg gehen und ein Pluginverzeichnis via FTP löschen
(insbesondere wenn das Plugin vor dem Entfernen der Dateien aktiv war)

### Custom Post Types

Installieren Sie das Plugin [Events Manager](http://wordpress.org/plugins/events-manager/) (oder ein anderes Veranstaltungskalender-Plugin, z. B. von [Modern Tribe](http://wordpress.org/plugins/the-events-calendar/). Erstellen Sie einen Veranstaltungsort und zwei bis vier Veranstaltungen.


### Theme auswählen / aktivieren / anpassen

Wählen Sie eines (oder nacheinander mehrere) der vorinstallierten Themes aus und aktivieren Sie es. Verändern Sie die Einstellungen und beobachten Sie das Resultat. Suchen Sie ein beliebiges Theme von wordpress.org/themes und installieren Sie es. Nutzen Sie den Customizer (Design/Anpassen) und vergleichen Sie die Möglichkeiten verschiedener Themes.

### Child Theme erstellen

Erstellen Sie ein (noch leeres) Child Theme Ihres aktiven Themes indem Sie im Dateisystem unter wp-content/themes/ einen neuen Ordner erstellen.
Erstellen Sie darin eine styles.css-Datei, zb. so:


![style.css des Child Themes(Beispiel) ](images/v4.5/child-style.png)

<<[style.css des Child Themes](code/child-style.css)


sowie eine (ebenfalls noch leere) functions.php

![functions.php des Child Themes (Beispiel)](images/v4.5/child-functions.png)

<<[functions.php des Child Themes](code/child-functions.php)


Oder wählen Sie die einfache Route und lassen Sie sich ein Child Theme online [WordPress Child Theme Generator](http://graphpaperpress.com/wordpress-child-theme-generator/)  erstellen.

Anschliessend können Sie die Zip-Datei wie ein normales Theme direkt via Backend hochladen.

Noch einfacher geht es mit Hilfe des Plugins [Child Theme Configurator](https://wordpress.org/plugins/child-theme-configurator/).

Mehr Infos zu Child Themes finden Sie im [Codex](ttp://codex.wordpress.org/Child_Themes) oder in meiner Präsentation auf [Speaker Deck](https://speakerdeck.com/zu).


### Themedateien bearbeiten

Die folgenden Aufgaben beziehen sich auf das TwentyThirteen Theme. In anderen Themes können die Dateien und CSS-Selektoren anders sein.

Entfernen Sie den Text "Proudly powered by WordPress" vollständig aus der Fusszeile (footer.php). Passen Sie das Stylesheet (style.css) an, um dem Seitentitel eine individuelle Farbe und einen Schlagschatten zu geben. (Nutzen Sie "Inspect Element" und den CSS3 Generator [CSS3.me](http://css3.me/)

{:lang="css",title=”CSS-Beispielcode aus style.css von TwentyThirteen}

    .site-description {
        font: 300 italic 24px "Source Sans Pro", Helvetica, sans-serif;
        margin: 0 0 0 32px;
    }
    
    .site-title { /* css3 Code ergänzen */ }

![Beispiel von Anpassungen durch Eingreifen in den CSS Code](images/v4.5/css3-seitentitel.png)
