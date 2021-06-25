---
layout: default
title: "curl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="curl">
  <a href="/de/common/curl.html">curl</a> <a href="#curl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Überträgt Daten von oder zu einem Server.
> Unterstützt die meisten Protokolle, inklusive HTTP, FTP und POP3.
> Weitere Informationen: <https://curl.se>.

#### Lade den Inhalt einer URL in eine Datei:
```shell
curl {{http://beispiel.de}} --output {{pfad/zu/datei}}
```
#### Lade eine Datei von einer URL herunter:
```shell
curl --remote-name {{http://beispiel.de/datei}}
```
#### Lade eine Datei herunter, folge Weiterleitungen und setze vergangene Dateitransfers automatisch fort:
```shell
curl --remote-name --location --continue-at - {{http://beispiel.de/datei}}
```
#### Sende formular-codierte Daten (POST Anfragen des Typs `application/x-www-form-urlencoded`). Benutze `--data @dateiname` oder `--data @'-'`, um von STDIN zu lesen:
```shell
curl --data {{'name=karl-dieter'}} {{http://beispiel.de/formular}}
```
#### Sende eine Anfrage mit einem extra Header mit einer eigenen HTTP-Methode:
```shell
curl --header {{'X-Mein-Header: 123'}} --request {{PUT}} {{http://beispiel.de}}
```
#### Sende Daten im JSON-Format und lege den geeigneten Inhaltstyp-Header fest:
```shell
curl --data {{'{"name":"karl-dieter"}'}} --header {{'Content-Type: application/json'}} {{http://beispiel.de/benutzer/1234}}
```
#### Übergib einen Benutzernamen und Passwort für die Server-Authentifizierung:
```shell
curl --user benutzername:passwort {{http://beispiel.de}}
```
#### Übergib Client-Zertifikat und -Schlüssel für eine Resource und überspringe die Zertifikatsüberprüfung:
```shell
curl --cert {{client.pem}} --key {{key.pem}} --insecure {{https://beispiel.de}}
```
{% endraw %}