## Mehrsprachigkeit in WordPress

Über 25% aller Internet-Auftritte basieren auf WordPress. Das Blog- und Content Management System ist enorm mächtig und fast in jeder Sprache erhältlich, sogar in Schwyzerdütsch[^Schwyzerdütsch].
Die Sprache von WordPress wird normalerweise während der Installation festgelegt. Dann wird die entsprechende Sprachdatei heruntergeladen und installiert. Später kann im Backend auf jede vorhandene Sprache gewechselt werden und sowohl Backend wie Frontend werden umgestellt. Natürlich betrifft das nicht den Inhalt selbst, sondern nur die Nutzungsoberfläche. Schaltflächen oder Links, wie “Weiterlesen…”, “Kategorie” etc. werden angepasst. Texte, welche von Themes oder Plugins eingefügt werden, kann WordPress nur übersetzen, wenn eine entsprechende Übersetzung vorhanden ist.

Gibt es keine Übersetzung in der entsprechenden Sprache, wird stattdessen die Standard-Sprache, also Englisch verwendet.
Dies ist unschön. Wurde als _Sprache der Website	_ beispielsweise _Deutsch (Sie)_ oder _Deutsch (Schweiz, Du)_ gewählt und gibt es keine entsprechende Übersetzung für ein Plugin oder Theme, wäre es wünschenswert der Fallback würde _Deutsch_ (also Standard-Deutsch) verwenden. So wie es jetzt aber implementiert ist, wird stattdessen die Standard-Englisch Übersetzung verwendet.

T>### Tipp
T>Das Plugin [Language Fallback](https://wordpress.org/plugins/language-fallback/) erlaubt es die (leider nur eine) Fallback-Sprache zu definieren.

### Sprachversion von WordPress ändern

Später lässt sich die Sprachversion immer noch ändern, indem im Backend unter Einstellungen / Allgemein die Sprache angepasst wird. WordPress lädt automatisch die zugehörigen Sprachdateien herunter und legt Sie im Ordner wp-content/languages ab. Für Themes und Plugins müssen unter Umständen weitere Sprachdateien installiert werden. 

Seit WordPress Version 3.7 werden Übersetzungen für Themes und Plugins automatisch von einem zentralen [Repository](https://translate.wordpress.org/) geladen und somit automatisch upgedatet. Die Übersetzungen werden im Ordner _wp_content/languages_ in einem Unterordner _themes_ bzw. _plugins_ mit dem _Slug [^Slug]_ des Plugin-Namens gespeichert. 

### WordPress für Mehrsprachigkeit vorbereiten

Standardmässig erscheint der gesamte Blog in einer einheitlichen Sprache. Wenn man Seiten und Beiträge in unterschiedlichen Sprachen anbieten möchte, geht das am einfachsten mit Hilfe eines Plugins.

Es gibt keinen “offiziellen” Weg die Sprache für einzelne Inhaltsbereiche festzulegen. Verschiedene Plugins erweitern WordPress daher auf unterschiedliche Weise um Mehrsprachigkeit zu ermöglichen:

1) Ein einzelner Beitrag oder eine Seite wird unterteilt in mehrere Sprachen.
— Vorteile: übersichtlich, einfach zu handhaben
— Nachteile: Beim Entfernen des Plugins enthalten einzelne Beiträge mehrere Sprachen. Das Entfernen einer Sprache wird somit sehr aufwändig.
— Beispiele: [Babble](https://github.com/Automattic/babble), [qTranslate X](https://wordpress.org/plugins/qtranslate-x/)

2) Beiträge haben jeweils korrespondierende Beiträge in anderen Sprachen. 
— Vorteile: Links auf eine spezifische Sprachversion eines Beitrags ist möglich. Es kann gut nur ein Teil der Webseite übersetzt werden.
— Nachteile: Benötigt eine “Hauptsprache”.
— Beispiel: [Polylang](https://wordpress.org/plugins/polylang), [WPML](https://wpml.org/de/)

3) Pro Sprache gibt es eine eigene WordPress-Instanz in einer Multisite.
— Vorteile: Sprachversionen sind unabhängig und können auch unter eigenen DOMAINs laufen.
— Nachteile: Benötigt Multisite, was schwieriger zu pflegen ist und nicht alle Plugins sind WordPress Multisite tauglich.
— Beispiel: [Multilingual Press](https://de.wordpress.org/plugins/multilingual-press/)

[^Schwyzerdütsch]: http://gsw.wordpress.org/ (nicht mehr aktiv)
[^Slug]: Der Slug ist die URL-taugliche Schreibweise des Beitragstitel, Plugin- oder Theme-Namen, also genau die Schreibweise, in ausschliesslich Kleinbuchstaben und ohne Sonderzeichen auch für den Ordnernamen des Themes oder Plugins verwendet wird.