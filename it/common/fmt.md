---
layout: default
title: "fmt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fmt">
  <a href="/it/common/fmt.html">fmt</a> <a href="#fmt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Riformatta i paragrafi di un file di testo unendoli e limitando la larghezza delle righe a un dato numero di caratteri (di default 75).
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/fmt>.

#### Riformatta un file:
```shell
fmt {{percorso/al/file}}
```
#### Riformatta un file producendo linee di (al massimo) `n` caratteri:
```shell
fmt -w {{n}} {{percorso/al/file}}
```
#### Riformatta un file senza unire assieme le linee più corte della data larghezza:
```shell
fmt -s {{percorso/al/file}}
```
#### Riformatta un file usando una spaziatura uniforme (1 spazio tra due parole e 2 spazi tra due paragrafi):
```shell
fmt -u {{percorso/al/file}}
```
{% endraw %}