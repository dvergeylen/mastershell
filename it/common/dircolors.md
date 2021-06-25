---
layout: default
title: "dircolors"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dircolors">
  <a href="/it/common/dircolors.html">dircolors</a> <a href="#dircolors"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Stampa comandi necessari per settare la variabile d'ambiente LS_COLOR per stilizzare `ls`, `dir`, etc.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/dircolors>.

#### Stampa i comandi per settare LS_COLOR con i colori predefiniti:
```shell
dircolors
```
#### Stampa i comandi per settare LS_COLOR con i colori definiti in un file:
```shell
dircolors {{file}}
```
#### Stampa comandi per la Bourne shell:
```shell
dircolors --bourne-shell
```
#### Stampa comandi per la C shell:
```shell
dircolors --c-shell
```
#### Mostra i colori predefiniti per diversi tipi di file ed estensioni:
```shell
dircolors --print-data
```
{% endraw %}