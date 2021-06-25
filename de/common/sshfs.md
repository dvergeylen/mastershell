---
layout: default
title: "sshfs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sshfs">
  <a href="/de/common/sshfs.html">sshfs</a> <a href="#sshfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Dateisystem Client für SSH.
> Weitere Informationen: <https://github.com/libfuse/sshfs>.

#### Hänge ein externes Verzeichnis ein:
```shell
sshfs {{benutzer}}@{{externer_server}}:{{externes_verzeichnis}} {{lokales_einhänge_verzeichnis}}
```
#### Hänge ein externes Verzeichnis aus:
```shell
umount {{lokaler_einhänge_verzeichnis}}
```
#### Hänge ein externes Verzeichnis unter einem bestimmten Port ein:
```shell
sshfs {{benutzer}}@{{externer_server}}:{{externes_verzeichnis}} -p {{2222}}
```
#### Verwende Komprimierung:
```shell
sshfs {{benutzer}}@{{externer_server}}:{{externes_verzeichnis}} -C
```
#### Folge symbolischen Links:
```shell
sshfs -o follow_symlinks {{benutzer}}@{{externer_server}}:{{externes_verzeichnis}} {{lokaler_einhänge_verzeichnis}}
```
{% endraw %}