#Tipps_und_Tricks

##Sicherheits-Tipps

WordPress an und für sich ist nicht aussergewöhnlich anfällig für Hackangriffe. Die weite Verbreitung von Webseiten auf WordPress Basis macht sie aber zu einem beliebten Ziel für solche. Die meisten erfolgreichen Angriffe funktionieren wegen der Missachtung einfacher Sicherheitsregeln, die nicht WordPress-spezifisch sind:

* schwache Passwörter
* unverschlüsselte FTP-Verbindungen
* Malware auf dem eigenen Computer.

Beim Aufsetzen Ihrer WordPress-Installation durch switchplus wurden bereits verschiedene Sicherheitsmassnahmen getroffen, einige davon sind:

* Löschen des Standard-Admin Kontos
* (Verwenden eines starken Passworts)
* Limitierung der Login-Versuche
* Filtern von Kommentar-Spam

Um die Sicherheit Ihres Internet-Auftritts zu erhalten sollten Sie:

* Keine Themes oder Plugins installieren, die nicht von vertrauenswürdigen Quellen stammen, vergl. [Quellen guter Themes](#anpassen_themesanbieter).

* Themes, Plugins und WordPress selbst immer auf dem aktuellsten Stand halten

Zusätzlich können Sie das Login ins Backend und die Administration Ihrer WordPress-Installation über eine verschlüsselte Verbindung erzwingen. Dazu müssen Sie in Ihrer wp_config.php Datei folgende Zeile irgendwo vor

{lang=php, title="wp_config.php", line-numbers=off }
	/* That's all, stop editing! Happy blogging. */ 

einfügen:

{lang=php, title="Verschlüsseltes Login und Dashboard erzwingen in wp_config.php", line-numbers=off }
    define('FORCE_SSL_ADMIN', true);