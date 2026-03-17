# Übung Aufbau-CMS

## Aufgabe 1:

1. Der User gibt https://supercms.ch im Browser ein.

2. Der Browser baut eine HTTPS-Verbindung zum Webserver auf.

3. Der Webserver empfängt die HTTPS-Anfrage auf Port 443.

4. Der Webserver greift auf das CMS im Verzeichnis /var/www/html/super-cms zu.

5. Der Webserver führt die PHP-Datei des CMS aus (z.B. index.php).

6. Das CMS lädt die Konfigurationsdatei database.php.

7. Über mysqli stellt das CMS eine Verbindung zum Datenbankserver her (IP 192.168.22.10, Port 3306).

8. Der Datenbankserver liest die Daten aus der Datenbank superCMS (Dateisystem ext4).

9. Die Daten werden zurück an den Webserver gesendet und als HTML-Seite über HTTPS an den Browser des Users geliefert.

---

## Aufgabe 2:

1. Der Administrator öffnet https://supercms.ch/phpmyadmin im Browser.

2. Der Browser baut eine HTTPS Verbindung zum Webserver auf.

3. Der Webserver empfängt die Anfrage für /phpmyadmin.

4. Der Webserver startet die phpMyAdmin Anwendung.

5. Der Administrator meldet sich bei phpMyAdmin an.

6. phpMyAdmin verbindet sich über mysqli mit dem Datenbankserver.

7. Die Verbindung erfolgt zum DB-Server 192.168.22.10 über Port 3306.

8. Der Administrator führt eine Änderung an der Datenbank superCMS aus.

9. Die Änderungen werden im Dateisystem ext4 des DB-Servers gespeichert.