---
layout: default
title: "deluged"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="deluged">
  <a href="/it/common/deluged.html">deluged</a> <a href="#deluged"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un processo demone per il client BitTorrent Deluge.
> Maggiori informazioni: <https://deluge-torrent.org>.

#### Avvia il demone di Deluge:
```shell
deluged
```
#### Avvia il demone di Deluge su di una specifica porta:
```shell
deluged -p {{porta}}
```
#### Avvia il demone di Deluge utilizzando uno specifico file di configurazione:
```shell
deluged -c {{percorso/a/file_configurazione}}
```
#### Avvia il demone di Deluge e scrivi il log in un file:
```shell
deluged -l {{percorso/a/file_log}}
```
{% endraw %}