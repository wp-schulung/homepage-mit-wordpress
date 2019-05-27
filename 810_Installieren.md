# Installieren

## Installieren auf dem switchplus-Hosting

### Grundkonfiguration

![Menü Grundkonfiguration/Bearbeiten Icon](images/screenshots/installieren-1.png)

Geben Sie als "Pfad auf dem Webspace oder Weiterleitungsziel"  den Pfad zu Ihrem Verzeichnis auf dem Server an und fügen Sie einen Ordner "wordpress" an. Dieser Ordner wird automatisch erstellt, falls Sie das Häkchen bei der Checkbox "Pfad anlegen" gesetzt haben. Andernfalls können Sie es über den Dateimanager erstellen.

![Pfad für WordPress in einem eigenen Verzeichnis](images/screenshots/installieren-2.png)

PHP-Edition: Einstellungen: Aktuelle, stabile PHP-Version auswählen.
PHP-Version: Standard verwenden

![PHP-Einstellungen](images/screenshots/installieren-3.png)

### Dateimanager

Mit Hilfe des switchplus Dateimanagers in Ihrem Benutzerkonto können Sie bequem Verzeichnisse erstellen und Dateien verwalten. Ein FTP-Zugang ist daher zum Installieren oder Anpassen einer WordPress Installation gar nicht nötig. 

### FTP-Zugang

Zwar ist FTP Zugang nicht zwingend erforderlich, da via Dateimanager die Dateimanipulationen ebenfalls möglich sind. Einen FTP-Account richten Sie über das Menü FTP-Zugang ein. Achten Sie darau, dass sie mit FTP den Pfad überhalb des wordpress Ordners anlegen.

![FTP Zugang anlegen](images/screenshots/installieren-6.png)

### MySQL-Datenbanken

Erstellen Sie eine Neue SQL-DB.
Datenbankname und Datenbankbenutzer sind identisch.
Das Passwort können Sie beim Erstellen frei wählen. (4-200 Zeichen).
Bei der Datenbankversion wählen Sie die aktuellste, stabile Version aus (im Moment MySQL 5.6)

Die ausgewählte Version entschiedet unter welcher Hostadresse die Datenbank angesprochen wird.
Dies ist im Normalfall mysql5.your-company.ch (wobei your-company.ch natürlich durch Ihren tatsächlichen Domainnamen ersetzt werden muss).

![MySQL Datenbank erstellen](images/screenshots/installieren-5.png)

![MySQL Datenbanken Übersicht](images/screenshots/installieren-4.png)

## Installieren auf dem lokalen Rechner (Windows, Mac, Linux)
(dieser Teil ist noch nicht vorhanden, sorry)