# Bedienen

## Übersicht über die Verwaltungsoberfläche

### Das Dashboard

![Das WordPress Dashboard](images/v4.5/dashboard.png)

Wenn man sich via **your-company.ch/wp-admin** in den Administrationsbereich von WordPress einloggt, landet man zuerst auf dem Dashboard. In den verschiedenen Modulen (z. B. "Auf einen Blick", "Aktivität", "WordPress Nachrichten") werden übersichtlich wichtige Informationen angezeigt. Wie auf allen anderen Administrationsseiten, die via das Menü auf der linken Seite ausgewählt werden können, lassen sich Module ein und ausblenden und zumindest auf der Dashboardseite auch fast beliebig anordnen. Dazu klickt man auf die unscheinbare Schaltfläche ”**Optionen**” oben rechts. Es erscheint eine Übersicht “**Boxes**”, in welcher die vorhandenen Module gecheckt werden können. Manche Module (und damit Informationen und/oder Einstellungsmöglichkeiten) werden durch Plugins hinzugefügt (im Screenshot beispielsweise "Cerber Schnellansicht").

Nicht ausgewählte Module verschwinden von der Seite. Die anderen lassen sich mittels Drag & Drop an eine beliebige Position verschieben und je nach individuellem Geschmack anordnen. Diese Einstellungen werden pro Benutzer gespeichert.

Die Module lassen sich durch Klick auf die Titelleiste minimieren und in manchen Fällen konfigurieren.

Auf vielen Seiten im Backend lassen sich Optionen einblenden und so die eingeblendeteten Spalten und die Anzahl Einträge pro Seite einstellen.

![Optionen für Beiträge](images/v4.5/optionen-beitraege.png)


## Hilfe

Ebenfalls oben rechts, direkt neben "Optionen einblenden" befindet sich eine kontextsensitive Hilfe. Die durch Klick eingeblendeten Hilfetexte beziehen sich daher immer auf die aktuelle Seite. In vielen Fällen gibt es zusätzlich weiterführende Links, die oft auf englischsprachige Webseiten verweisen.

![Hilfe für Beiträge](images/v4.5/hilfe-beitraege.png)


### Die Adminleiste

Die Adminleiste ist im Backend und für angemeldete Benutzer auch im Frontend sichtbar.

![Adminleiste im Backend...](images/v4.5/admin-leiste-backend.png)

![... und im Frontend](images/v4.5/admin-leiste-frontend.png)

{float=left}
![](images/v4.5/adminbar-w.png)

Unter dem WordPress Icon befindet sich "Über WordPress". Hier gibt es Informationen zur aktuell installierten Version. Darunter befinden sich Links zur Dokumentation und den Benutzerforen, wo man Hilfe erhalten kann.

{float=left}
![](images/v4.5/seitenname-front.png)

Wenn man mit der Maus über den Seitenamen (my-company.ch) fährt öffnet sich ein Dropdownmenü. Im Backend mit einem einzigen Eintrag "Zur Seite". Im Frontend befinden sich dort Links zu unterschiedlichen Bereichen im Backend. Ein Klick auf den Namen selbst führt direkt ins Backend bzw. aus dem Backend zurück zum Frontend.

"Die Sprechblase" zeigt an, wieviele Kommentare auf die Moderation warten und führt direkt zu dem Bereich im Backend, wo Kommentare freigeschaltet, zurückgewiesen oder auch beantwortet werden können.

"+Neu" erlaubt das Erfassen eines neuen Artikels, einer neuen Seite oder eines zusätzlichen Benutzers, sowie das Hochladen von Dateien in die Mediathek. Themes oder Plugin können zusätzliche Inhaltstypen bereitstellen, welche dann ebenfalls von hier erstellt werden können (Custom Post Types).


{float=left}
![](images/v4.5/admin-leiste-updates.png)

Ebenfalls in der Adminleiste wird angezeigt, wie viele Updates anstehen.
Dies sind neue Versionen von WordPress selber, Themes oder Plugins.
Ein Klick auf das Symbol führt zu einer Seite, die übersichtlich auflistet, was alles per Klick automatisch upgedatet werden kann.

![Übersicht über vorhandene Updates](images/v4.5/updates.png)

Ebenfalls wird direkt bei den Plugins und Themes angezeigt, wie viele davon in einer neuen Version vorhanden sind.

Ich empfehle, immer auf die neueste Version upzudaten. Möglicherweise wurden entdeckte Sicherheitslücken geschlossen. Verharren auf der "alten" Version macht die Webseite dann "verletzlich" für Hacker-Angriffe.


### Allgemeine Einstellungen vornehmen
In WordPress lassen sich diverse grundlegende "Einstellungen" konfigurieren. Die Anpassungen betreffen dabei:

#### Allgemein
	- Seitentitel, Untertitel, URLs, E-Mail-Adresse für Benachrichtigungen
	- Mitgliedschaft / Benutzerverwaltung
	- Zeitformat/Datumsformat --> Beitragsmetainformationen
	- Sprache

#### Schreiben
	- Formatierung (Emoticons, XHTML-Code)
	- Standardkategorie /-formatvorlage für Beiträge
	- Via E-Mail schreiben (evtl. andere Kategorie)
	- Update Services (abhängig von Sichtbarkeitseinstellungen --> Lesen)

#### Lesen
	- Startseite (Blog, statische Seite), Anzahl Beiträge, Suchmaschinen

#### Diskussion
	- Pingbacks und Trackbacks
	- Kommentareinstellungen und Avatare

#### Medien
	- Bildgrössen (bei Änderung müssen bestehende Bilder neu berechnet werden. Plugin: [Regenerate Thumbnails](http://wordpress.org/plugins/regenerate-thumbnails/) )
	- Ordnerorganisation (Uploads in monats- und jahresbasierten Ordnern. Empfehlung: deaktivieren)

#### Permalinks
	- Einstellung der URL-Struktur für Permalinks (.htaccess Datei wird - sofern möglich - automatisch geschrieben)
    - Kategorie- und Schlagwortbasis (also die Bezeichnung, Archivseiten vorausgeht)
    
T>### Tipp
T>Wenn nach einer Migration oder Änderung der Installation Links nicht mehr funktionieren: Permalinks neu speichern!

Plugins (und manchmal auch Themes) erstellen oft eigene Menüpunkte.

### Artikel oder Seiten erstellen und bearbeiten mit dem Editor
Wenn man im Menü links Artikel oder Seiten auswählt, erscheint die Übersicht bereits bestehender Artikel bzw. Seiten.
Ganz oben, rechts vom Titel, hat es eine Schaltfläche "Erstellen". Diese führt, genauso, wie die Auswahl "Erstellen" im Menü, zum Editor, in welchem Titel und Inhalt des Artikels oder der Seite erfasst werden können.

Zwischen dem Visuellen Editor und einem Text-Editor kann einfach hin- und her gewechselt werden.

![Visueller Editor](images/v4.5/visueller-editor.png)

![Code Editor](images/v4.5/text-editor.png)

Die Bedienung des visuellen und HTML-Editors werden in der **WordPress-Anleitung für Autoren & Redakteure** detailliert beschrieben.
Teilnehmer einer Schulung bei switchplus können die passwortgeschützte Datei kostenlos von
[switchie.ch/schulungsunterlagen/](https://switchie.ch/schulungsunterlagen/)
herunterladen.

Die Kaufversion gibt es direkt beim Autor [Perun (Vladimir Simovi&#263; auf www.perun.net)](http://www.perun.net/wordpress-administratoren/)

In der Übersichtsansicht lässt sich ein Beitrag bzw. eine Seite zum Editieren auswählen in dem man "Editieren" anklickt, welches bei MouseOver sichtbar wird. Ausserdem lassen sich die Artikel und Seiten nach Spalte sortieren indem auf der Titelleiste auf den entsprechende Titel geklickt wird. Artikel und Seiten können via das Suchfeld oben rechts gefunden oder mit Hilfe der Filterfunktionen eingeschränkt werden.
Bei einer grossen Anzahl einzelner Artikel oder Seiten werden diese auf mehrere Seiten verteilt. Obwohl Sortierung und Filter sich auf die gesamten Artikel und Seiten auswirken und nicht nur auf die aktuell angezeigten, möchte man sich vielleicht eine grössere Liste anzeigen lassen. Dies lässt ich über das Einblenden der Optionen bewerkstelligen.

X>## Übungen: [Einstellungen](#ueb-einstellungen-vornehmen) / [Beiträge erfassen](#ueb-beitraege-erfassen) / [Beitrag (Standard) formatieren](#ueb-beitraege-formatieren) / [Kategorien und/oder Schlagworte nutzen](#ueb-kategorien-tags)
X>
X> Um das bisher gelernte praktisch anwenden zu können, finden Sie im [letzten Teil](#teil-2) des Buches Übungen.

