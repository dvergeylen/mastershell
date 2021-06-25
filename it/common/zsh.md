---
layout: default
title: "zsh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zsh">
  <a href="/it/common/zsh.html">zsh</a> <a href="#zsh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Z SHell.
> Inteprete da linea di comando compatibile con `bash` e `sh`.
> Maggiori informazioni: <https://www.zsh.org>.

#### Fai partire l'interprete interattivo da linea di comando:
```shell
zsh
```
#### Esegui un comando passandolo come parametro:
```shell
zsh -c {{comando}}
```
#### Esegui comandi da un file (script):
```shell
zsh {{file}}
```
#### Esegui comandi da un file e stampali a schermo mentre vengono eseguiti:
```shell
zsh -x {{file}}
```
{% endraw %}