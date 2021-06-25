---
layout: default
title: "deluge-console"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="deluge-console">
  <a href="/it/common/deluge-console.html">deluge-console</a> <a href="#deluge-console"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interfaccia interattiva da linea di comando per il client BitTorrent Deluge.
> Maggiori informazioni: <https://deluge-torrent.org>.

#### Avvia un'interfaccia interattiva da console:
```shell
deluge-console
```
#### Connetti ad un'instanza del demone di Deluge:
```shell
connect {{hostname}}:{{porta}}
```
#### Aggiungi un torrent al demone:
```shell
add {{url|magnet|percorso/a/file}}
```
#### Mostra informazioni su tutti i torrent:
```shell
info
```
#### Mostra informazioni su di uno specifico torrent:
```shell
info {{id_torrent}}
```
#### Metti in pausa un torrent:
```shell
pause {{id_torrent}}
```
#### Riprendi un torrent:
```shell
resume {{id_torrent}}
```
#### Rimuovi un torrent dal demone:
```shell
rm {{id_torrent}}
```
{% endraw %}