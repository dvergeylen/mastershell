---
layout: default
title: "enca"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="enca">
  <a href="/it/common/enca.html">enca</a> <a href="#enca"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rileva e converti l'encoding di file di testo.
> Maggiori informazioni: <https://github.com/nijel/enca>.

#### Rileva l'encoding di uno o più file in base alla locale di sistema:
```shell
enca {{file1 file2 ...}}
```
#### Rileva l'encoding specificando un linguaggio nel formato di locale POSIX/C (e.g. zh_CN, en_US):
```shell
enca -L {{linguaggio}} {{file1 file2 ...}}
```
#### Converti file ad uno specifico encoding:
```shell
enca -L {{linguaggio}} -x {{encoding}} {{file1 file2 ...}}
```
#### Crea una copia di un file esistente utilizznado un encoding diverso:
```shell
enca -L {{linguaggio}} -x {{encoding_finale}} < {{file_originale}} > {{nuovo_file}}
```
{% endraw %}