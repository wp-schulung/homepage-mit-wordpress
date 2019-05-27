# WordPress bei switchplus.ch einrichten

## Benutzerkonto eröffnen
Eröffnen Sie unter der Adresse [www.switchplus.ch](https://www.switchplus.ch) ein neues Benutzerkonto oder melden Sie sich an ein bestehendes Konto an.

## Installieren auf dem switchplus-Hosting

## Grundkonfiguration
Starten Sie die Bearbeitung des Domain-Namen im Hauptmenu unter **Produkte verwalten / Grundkonfiguration** durch Klick auf das **Bearbeiten-Symbol**  ganz rechts beim Domain-Namen.

![Menü Grundkonfiguration/Bearbeiten Icon](images/screenshots/installieren-1.png)

Geben Sie als "Pfad auf dem Webspace oder Weiterleitungsziel"  den Pfad zu Ihrem Verzeichnis auf dem Server an und fügen Sie einen Ordner "wordpress" an. Dieser Ordner wird automatisch erstellt, falls Sie das Häkchen bei der Checkbox "Pfad anlegen" gesetzt haben. Andernfalls können Sie es über den Dateimanager erstellen.

![Pfad für WordPress in einem eigenen Verzeichnis](images/screenshots/installieren-2.png)

Im Register **Einstellungen**  stellen Sie die **PHP-Edition** auf die höchste "Stable" Version (z. B. 5-56STABLE (5.6.0). Bei **PHP-Version** nutzen Sie auf **STANDARD** und klicken dann auf **speichern**.

![PHP-Einstellungen](images/screenshots/installieren-3.png)

![Grundkonfiguration/Allgemein](images/screenshots-probeabo/screenshot_05.jpg)

![Grundkonfiguration/Einstellungen](images/screenshots-probeabo/screenshot_06.png)

## MySQL-Datenbank
WordPress benötigt eine Datenbank. Sie können diese im Benutzerkonto mit dem Befehl **MySQL-Datenbanken** und **Neue SQL-DB** erstellen.

![MySQL-Datenbank erstellen](images/screenshots-probeabo/screenshots-mysql.png)

Der Name und das eben erstellte Passwort der Datenbank brauchen Sie später.
Darum kopieren Sie es jetzt am Besten in eine Textdatei.

### MySQL-Datenbanken

Erstellen Sie eine Neue SQL-DB.
Datenbankname und Datenbankbenutzer sind identisch.
Das Passwort können Sie beim Erstellen frei wählen. (4-200 Zeichen).
Bei der Datenbankversion wählen Sie die aktuellste, stabile Version aus (im Moment MySQL 5.6)

Die ausgewählte Version entschiedet unter welcher Hostadresse die Datenbank angesprochen wird.
Dies ist im Normalfall mysql5.your-company.ch (wobei your-company.ch natürlich durch Ihren tatsächlichen Domainnamen ersetzt werden muss).

![MySQL Datenbank erstellen](images/screenshots/installieren-5.png)

![MySQL Datenbanken Übersicht](images/screenshots/installieren-4.png)

## WordPress herunterladen
Laden Sie die aktuelle WordPress Version von http://de.wordpress.org/ herunter.

## FTP-Zugang oder Dateimanager
Die Installationsdateien von WordPress müssen auf den Server gelangen.
Dazu erstellen Sie einen **Neuen Account** unter **FTP-Zugang** oder nutzen den integrierten Dateimanager.

### Dateimanager

Mit Hilfe des switchplus Dateimanagers in Ihrem Benutzerkonto können Sie bequem Verzeichnisse erstellen und Dateien verwalten. Ein FTP-Zugang ist daher zum Installieren oder Anpassen einer WordPress Installation gar nicht nötig. 

![WordPress über Dateimanager hochladen](images/screenshots-probeabo/screenshot-hochladen.png)

Zip-Datei direkt auf dem Server entpacken und anschliessend verschieben.

![Dateien entpacken und verschieben](images/screenshots-probeabo/verschieben.png)

Wenn Sie nun die WordPressdateien am richtigen Ort auf dem Server haben, können Sie direkt über den Browser die Instalationsroutine starten indem Sie Ihre DOMAIN aufrufen.

### FTP-Zugang

Zwar ist FTP Zugang nicht zwingend erforderlich, da via Dateimanager die Dateimanipulationen ebenfalls möglich sind. Einen FTP-Account richten Sie über das Menü FTP-Zugang ein. Achten Sie darau, dass sie mit FTP den Pfad überhalb des wordpress Ordners anlegen.

![FTP Zugang anlegen](images/screenshots/installieren-6.png)

### Installationsroutine

![Konfigurationsdatei erstellen](images/screenshots-probeabo/install-1.png)

Im übernächsten Schritt müssen die Angaben der Datenbank eingetragen werden.

![MySQL-Datenbank Daten eingaben](images/screenshots-probeabo/install-2.png)

![Bloginformationen erfassen](images/screenshots-probeabo/install-3.png)

## Installieren auf dem lokalen Rechner (Windows, Mac, Linux)
(dieser Teil ist noch nicht vorhanden, sorry)