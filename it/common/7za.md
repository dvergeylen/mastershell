---
layout: default
title: "7za"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="7za">
  <a href="/it/common/7za.html">7za</a> <a href="#7za"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Archiviatore di file con alto fattore di compressione.
> Versione standalone di `7z` con supporto a meno tipi di archivi.
> Maggiori informazioni: <https://www.7-zip.org/>.

#### Archivia un file o una directory:
```shell
7za a {{archivio.7z}} {{percorso/a/file_o_directory}}
```
#### Estrai un archivio mantenendo la gerarchia delle cartelle:
```shell
7za x {{archivio.7z}}
```
#### Archivia utilizzando uno specifico tipo di archivio:
```shell
7za a -t {{zip|gzip|bzip2|tar}} {{archivio.7z}} {{percorso/a/file_o_directory}}
```
#### Elenca i tipi di archivio supportati:
```shell
7za i
```
#### Elenca i contenuti in un archivio:
```shell
7za l {{archivio}}
```
{% endraw %}