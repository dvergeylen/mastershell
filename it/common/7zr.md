---
layout: default
title: "7zr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="7zr">
  <a href="/it/common/7zr.html">7zr</a> <a href="#7zr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Archiviatore di file con alto fattore di compressione.
> Versione standalone di `7z` che supporta solo file .7z.
> Maggiori informazioni: <https://www.7-zip.org/>.

#### Archivia un file o una directory:
```shell
7zr a {{archivio.7z}} {{percorso/a/file_o_directory}}
```
#### Estrai un archivio mantenendo la gerarchia delle directory:
```shell
7zr x {{archivio.7z}}
```
#### Elenca i contenuti in un archivio:
```shell
7zr l {{archivio}}
```
{% endraw %}