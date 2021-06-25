---
layout: default
title: "ssh-keygen"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ssh-keygen">
  <a href="/de/common/ssh-keygen.html">ssh-keygen</a> <a href="#ssh-keygen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generiert ssh Schlüssel für Authentifizierung, Passwort-lose Logins und mehr.

#### Erstelle ein SSH Schlüssel-Paar interaktiv:
```shell
ssh-keygen
```
#### Erstelle ein Schlüssel-Paar unter einem bestimmten Dateinamen:
```shell
ssh-keygen -f ~/.ssh/{{datei}}
```
#### Generiere ein ed25519 Schlüssel-Paar mit 100 Schlüssel-Ableitungs-Iterationen:
```shell
ssh-keygen -t ed25519 -a 100
```
#### Generiere ein 4096 Bit langen RSA Schlüssel-Paar mit der Email im Kommentarfeld:
```shell
ssh-keygen -t rsa -b 4096 -C "{{email}}"
```
#### Rufe den Schlüssel-Fingerabdruck von einem Server ab (hilfreich um die Authentizität eines Servers beim ersten Verbinden zu überprüfen):
```shell
ssh-keygen -l -F {{externer_server}}
```
#### Entferne den Schlüssel eines Servers aus der `known_hosts` Datei (hilfreich wenn ein Server seinen Schlüssel aktualisiert hat und der alte somit nicht mehr gilt):
```shell
ssh-keygen -R {{externer_server}}
```
#### Rufe den Fingerabdrucks eines Schlüssels im MD5 Hex Format ab:
```shell
ssh-keygen -l -E md5 -f ~/.ssh/{{datei}}
```
#### Ändere das Passwort eines privaten Schlüssels:
```shell
ssh-keygen -p -f ~/.ssh/{{datei}}
```
{% endraw %}