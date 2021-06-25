---
layout: default
title: "sshpass"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sshpass">
  <a href="/de/common/sshpass.html">sshpass</a> <a href="#sshpass"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Stelle SSH Passwörtern bereit.

#### Stelle eine Verbindung zu einem externen Server über ein Passwort aus einem Datei-Objekt her (in diesem Fall stdin):
```shell
sshpass -d {{0}} ssh {{benutzer}}@{{server}}
```
#### Stelle eine Verbindung zu einem externen Server mit Hilfe eines Passworts bei automatischer Akzeptierung von unbekannten SSH Schlüsseln her:
```shell
sshpass -p {{passwort}} ssh -o StrictHostKeyChecking=no {{benutzer}}@{{server}}
```
#### Stelle eine Verbindung zu einem externen Server mit Hilfe eines Passworts aus der ersten Zeile einer Datei bei automatischer Akzeptierung von unbekannten SSH Schlüsseln mit anschließender Ausführung eines Befehls her:
```shell
sshpass -f {{pfad/zu/datei}} ssh -o StrictHostKeyChecking=no {{benutzer}}@{{server}} "{{befehl}}"
```
{% endraw %}