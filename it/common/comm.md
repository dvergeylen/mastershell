---
layout: default
title: "comm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="comm">
  <a href="/it/common/comm.html">comm</a> <a href="#comm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Seleziona o ignora linee comuni a due file. Entrambi i file devono essere ordinati.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/comm>.

#### Produci tre colonne separate da tab: linee solo nel primo file, linee solo nel secondo file, e linee comuni ad entrambi:
```shell
comm {{file1}} {{file2}}
```
#### Stampa solo le linee comune ad entrambi i file:
```shell
comm -12 {{file1}} {{file2}}
```
#### Stampa solo le lin comuni ad entrambi i file, leggendone uno da standard input:
```shell
cat {{file1}} | comm -12 - {{file2}}
```
#### Filtra le linee trovate solo nel primo file, salvando il risultato in un terzo file:
```shell
comm -23 {{file1}} {{file2}} > {{file3}}
```
#### Filtra le linee trovate solo nel secondo file, con due file che non sono ordinati:
```shell
comm -13 <(sort {{file1}}) <(sort {{file2}})
```
{% endraw %}