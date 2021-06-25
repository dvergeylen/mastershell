---
layout: default
title: "aria2"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aria2">
  <a href="/it/common/aria2.html">aria2</a> <a href="#aria2"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumento di download da linea di comando leggero, multi-protocollo e multi-sorgente.
> Supporta HTTP, HTTPS, FTP, SFTP, BitTorrent e Metalink.
> Maggiori informazioni: <https://aria2.github.io/>.

#### Scarica una risorsa web:
```shell
aria2c {{http://example.org/myLinux.iso}}
```
#### Scarica una risorsa da sorgenti multiple:
```shell
aria2c {{http://mirror1.org/myLinux.iso}} {{http://mirror2.org/myLinux.iso}}
```
#### Scarica utilizzando 2 connessioni per host:
```shell
aria2c -x{{2}} {{http://example.org/myLinux.iso}}
```
#### Scarica un file da un URI Metalink:
```shell
aria2c {{http://example.org/myLinux.metalink}}
```
#### Scarica da un URI BitTorrent:
```shell
aria2c {{http://example.org/myLinux.torrent}}
```
#### Scarica da un Magnet URI BitTorrent:
```shell
aria2c {{'magnet:?xt=urn:btih:248D0A1CD08284299DE78D5C1ED359BB46717D8C'}}
```
#### Scarica dagli URI listati in un file:
```shell
aria2c -i {{uris.txt}}
```
{% endraw %}