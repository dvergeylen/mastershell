---
layout: default
title: "aria2c"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aria2c">
  <a href="/it/common/aria2c.html">aria2c</a> <a href="#aria2c"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Veloce utilità di download.
> Supporta HTTP(S), FTP, SFTP, BitTorrent, e Metalink.
> Maggiori informazioni: <https://aria2.github.io>.

#### Scarica un file da un URI:
```shell
aria2c {{url}}
```
#### Scarica più file da diverse sorgenti:
```shell
aria2c {{url_1}} {{url_2}}
```
#### Scarica gli URI elencati in un file:
```shell
aria2c -i {{filename}}
```
#### Esegui il download con connessioni multiple:
```shell
aria2c -s {{numero_connessioni}} {{url}}
```
#### Scarica via FTP con username e password:
```shell
aria2c --ftp-user={{username}} --ftp-passwd={{password}} {{url}}
```
#### Limita la valocità di download (in byte al secondo):
```shell
aria2c --max-download-limit={{velocità}} {{url}}
```
{% endraw %}