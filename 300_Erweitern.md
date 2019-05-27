{#erweitern}
# Erweitern

## Plugins
Erweitern lässt sich WordPress in erster Linie über Plugins.
Da Plugins tief ins System eingreifen können, sind mächtige Anpassungen möglich. Das führt unter Umständen dazu, dass ein Plugin Schaden anrichtet oder Sicherheitslücken öffnet. Wir empfehlen dringend, Plugins (wie auch Themes) nur aus offiziellen bzw. vertrauenswürdigen Quellen zu beziehen. Plugins lassen sich am einfachsten direkt über das Backend installieren.

![Übersicht über die installierten Plugins im Backend. Installieren klicken um weitere Plugins zu installieren.](images/v4.5/plugin-aktualisieren.png)

Installierte Plugins lassen sich Aktivieren/Deaktivieren und, falls eine neue Version vorhanden ist, aktualisieren. Deaktivierte Plugins kann man löschen. So werden Sie vollständig vom Server entfernt. Einstellungen bleiben gewöhnlich in der Datenbank bestehen.

![Die Auswahl an Plugins ist riesig. Die Suche nach einem geeigneten nicht immer einfach.](images/v4.5/plugin-installieren.png)

Die Filter **Vorgestellt**, **Populär** und **Empfohlen** zeigen jeweils unterschiedliche Plugins. Besonders interessant ist dabei **Empfohlen**. Hier macht WordPress Vorschläge aufgrund der bereits installierten Plugins.

Alternativ (und manchmal bei kostenpflichtigen Plugins nötig) lassen sich Plugins auch über das Backend hochladen. Dafür lässt sich die komplette Plugin-Zip-Datei direkt im Backend auswählen und hochladen und anschliessend aktivieren. Als dritte Möglichkeit lassen sich Plugins auch via FTP (oder den switchplus Dateimanager) in den WordPress Ordner **/wp-content/plugins/** auf dem Server kopieren.
Danach stehen sie im Backend bereit und können von dort aktiviert werden.

T>### Tipp
T>Wenn ein Plugin Ursache für ein nicht mehr bedienbares WordPress ist und man sich nicht mehr im Backend einloggen kann, lässt sich der Plugin Ordner des Plugins, welches den Fehler verursacht, direkt vom Server löschen (oder umbenennen). WordPress deaktiviert das fehlende Plugin dann automatisch.

## Custom Post Types
Custom Post Types lassen sich manuell erstellen. Dazu muss man Code schreiben. Es gibt Tools um sich den Code erstellen zu lassen, z. B.

- [GenerateWP](http://generatewp.com/post-type/).

Der durch den Generator erstellten Code müssen Sie entweder in die _functions.php_ Datei des aktiven (Child-)Themes kopieren oder in ein eigenes Plugin. Diese fortgeschrittenen Techniken sind jedoch kein Bestandteil in diesen Kurs-Unterlagen.

Die folgenden Hinweise zum Codex[^codex] und zu spezialisierten Plugins, die es ermöglichen ohne Eingriff in den Code tiefgreifende Anpassungen in WordPress vorzunehmen und Custom Post Types mitsamt zugehöriger Zusatzfelder zu erstellen, dienen daher lediglich als Anhaltspunkt für interessierte oder potentielle Theme-Entwickler.

[^codex]:Der WordPress Codex ist das Online Manual zu WordPress und zusammen mit der [Code Referenz](https://developer.wordpress.org/reference/) die wichtigste Informationsquelle zur Theme- und Plugin-Entwicklung

Weitere Informationen zu Custom Post Types findet man im WordPress Codex: [Post Types](http://codex.wordpress.org/Post_Types)

Mit Hilfe von Plugins, wie [Advanced Custom Fields](https://wordpress.org/plugins/advanced-custom-fields/), [CMB2](https://wordpress.org/plugins/cmb2/), [Custom Field Suite](https://wordpress.org/plugins/custom-field-suite/) oder [WCK - Custom Fields and Custom Post Types Creator](https://wordpress.org/plugins/wck-custom-fields-and-custom-post-types-creator/) (neben vielen anderen) ist es jedoch möglich über das WordPress Backend eigene Inhaltstypen zu erstellen. Um diese im Frontend darzustellen, müssen Sie Templatedateien des genutzten Themes anpassen.
Bei _WCK - Custom Fields and Custom Post Types Creator_ ist es möglich den benötigten Code direkt im Backend via Copy & Paste einzugeben.


