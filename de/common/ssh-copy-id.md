---
layout: default
title: "ssh-copy-id"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ssh-copy-id">
  <a href="/de/common/ssh-copy-id.html">ssh-copy-id</a> <a href="#ssh-copy-id"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Installiere den öffentlichen Teil eines SSH Schlüssels in der `authorized_keys` Datei auf einem externen Server.

#### Kopiere den eigenen öffentlichen SSH Schlüssels zu einem externen Server:
```shell
ssh-copy-id {{benutzer}}@{{externer_server}}
```
#### Kopiere den angegebenen öffentlichen SSH Schlüssels zu einem externen Server:
```shell
ssh-copy-id -i {{pfad/zu/öffentlichem_schlüssel}} {{benutzer}}@{{externer_server}}
```
#### Kopiere den angegeben öffentlichen SSH Schlüssels zu einem externen Server unter Angabe eines bestimmten SSH Ports:
```shell
ssh-copy-id -i {{pfad/zu/öffentlichem_schlüssel}} -p {{port}} {{benutzer}}@{{externer_server}}
```
{% endraw %}