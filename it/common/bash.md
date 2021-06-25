---
layout: default
title: "bash"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bash">
  <a href="/it/common/bash.html">bash</a> <a href="#bash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bourne-Again SHell.
> Interprete da linea di comando compatibile con `sh`.
> Maggiori informazioni: <https://gnu.org/software/bash>.

#### Avvia una shell interattiva:
```shell
bash
```
#### Esegui un comando:
```shell
bash -c "{{comando}}"
```
#### Esegui dei comandi da un file:
```shell
bash {{file.sh}}
```
#### Esegui dei comandi da un file, loggando tutti i comandi eseguiti nel terminale:
```shell
bash -x {{file.sh}}
```
#### Esegui comandi da standard input:
```shell
bash -s
```
#### Stampa informazioni sulla versione di bash (usa `echo $BASH_VERSION` per mostrare solo la versione):
```shell
bash --version
```
{% endraw %}