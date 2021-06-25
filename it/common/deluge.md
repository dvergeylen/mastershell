---
layout: default
title: "deluge"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="deluge">
  <a href="/it/common/deluge.html">deluge</a> <a href="#deluge"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Client BItTorrent da linea di comando.
> Maggiori informazioni: <https://deluge-torrent.org>.

#### Scarica un torrent:
```shell
deluge {{url|magnet|percorso/a/file}}
```
#### Scarica un torrent utilizzando uno specifico file di configurazione:
```shell
deluge -c {{percorso/a/file_configurazione}} {{url|magnet|percorso/a/file}}
```
#### Scarica un torrent ed avvia una specifica interfaccia utente:
```shell
deluge -u {{gtk|web|console}} {{url|magnet|percorso/a/file}}
```
#### Scarica un torrent e scrivi il log in un file:
```shell
deluge -l {{percorso/a/file_log}} {{url|magnet|percorso/a/file}}
```
{% endraw %}