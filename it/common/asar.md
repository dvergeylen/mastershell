---
layout: default
title: "asar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="asar">
  <a href="/it/common/asar.html">asar</a> <a href="#asar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestore di archivi per la piattaforma Electron.
> Maggiori informazioni: <https://github.com/electron/asar>.

#### Archivia un file o una cartella:
```shell
asar pack {{percorso/al/file}} {{archivio.asar}}
```
#### Estrai un archivio:
```shell
asar extract {{archivio.asar}}
```
#### Estrai uno specifico file da un archivio:
```shell
asar extract-file {{archivio.asar}} {{nome_file}}
```
#### Elenca i contenuti in un archivio:
```shell
asar list {{archivio.asar}}
```
{% endraw %}