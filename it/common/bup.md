---
layout: default
title: "bup"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bup">
  <a href="/it/common/bup.html">bup</a> <a href="#bup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sistema di backup basato sul formato dei packfile Git, fornendo salvataggi incrementali veloci e deduplicazione globale.
> Maggiori informazioni: <https://github.com/bup/bup>.

#### Inizializza una repository di backup nella directory locale specificata:
```shell
bup -d {{percorso/a/repository}} init
```
#### Prepara una certa cartella prima di fare un backup:
```shell
bup -d {{percorso/a/repository}} index {{percorso/a/directory}}
```
#### Esegui il backup di una cartella in una repository locale:
```shell
bup -d {{percorso/a/repository}} save -n {{nome_backup}} {{percorso/a/directory}}
```
#### Elenca i di backup attualmente nella repository:
```shell
bup -d {{percorso/a/repository}} ls
```
#### Ripristina uno specifico backup in una determinata cartella locale:
```shell
bup -d {{percorso/a/repository}} restore -C {{percorso/a/destinazione}} {{nome_backup}}
```
{% endraw %}