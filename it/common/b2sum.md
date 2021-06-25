---
layout: default
title: "b2sum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="b2sum">
  <a href="/it/common/b2sum.html">b2sum</a> <a href="#b2sum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Calcola checksum BLAKE2.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/b2sum>.

#### Calcola il checksum BLAKE2 per un file:
```shell
b2sum {{file1}}
```
#### Calcola checksum BLAKE2 per più file:
```shell
b2sum {{file1}} {{file2}}
```
#### Leggi un file di checksum BLAKE2 e nomi di file e verifica che tutti i file abbiano lo stesso checksum:
```shell
b2sum -c {{elenco_checksum.b2}}
```
#### Calcola il checksum BLAKE2 da standard input:
```shell
{{comando}} | b2sum
```
{% endraw %}