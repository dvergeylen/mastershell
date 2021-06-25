---
layout: default
title: "ssh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ssh">
  <a href="/de/common/ssh.html">ssh</a> <a href="#ssh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Secure Shell ist ein Protokoll für das sichere einloggen auf einem externen System.
> Es kann dafür eingesetzt werden um Befehle auf externen Systemen auszuführen.

#### Stelle eine Verbindung zu einem externen Server her:
```shell
ssh {{benutzer}}@{{externer_server}}
```
#### Stelle eine Verbindung zu einem externen Server mit spezifischer Identität her (privater SSH Schlüssel):
```shell
ssh -i {{pfad/zu/schlüssel_datei}} {{benutzer}}@{{externer_server}}
```
#### Stelle eine Verbindung zu einem externen Server unter einem spezifischen Port her:
```shell
ssh {{benutzer}}@{{externer_server}} -p {{2222}}
```
#### Führen einen Befehl auf einem externen Server aus:
```shell
ssh {{externer_server}} {{befehl}}
```
#### SSH Tunneln: Leite Ports dynamische Port weiter (SOCKS proxy auf localhost:1080):
```shell
ssh -D {{1080}} {{benutzer}}@{{externer_server}}
```
#### SSH Tunneln: Leite einen spezifischen Ports (localhost:9999 zu example.org:80) weiter zusammen mit deaktivierter pseudy-tty Provisionierung für die Ausführung eines Befehls:
```shell
ssh -L {{9999}}:{{example.org}}:{{80}} -N -T {{benutzer}}@{{externer_server}}
```
#### SSH Springen: Verbinde über einen Spring-Server zu einem externen Server (Es können auch mehrere Spring-Server über eine Komma-separierte Liste angegeben werden):
```shell
ssh -J {{benutzer@sring_server}} {{benutzer}}@{{externer_server}}
```
#### Agenten Weiterleitung: Leite ie eigenen Authentifizierungs-Information an den externen Server weiter (siehe `man ssh_config` für mehr Optionen):
```shell
ssh -A {{benutzer}}@{{externer_server}}
```
{% endraw %}