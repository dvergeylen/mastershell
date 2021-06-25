---
layout: default
title: "mv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mv">
  <a href="/it/common/mv.html">mv</a> <a href="#mv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sposta o rinomina file e directory.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/mv>.

#### Sposta file:
```shell
mv {{sorgente}} {{destinazione}}
```
#### Sposta file senza chiedere conferma prima di sovrascrivere file esistenti:
```shell
mv -f {{sorgente}} {{destinazione}}
```
#### Sposta file interattivamente, chiedendo conferma prima di sovrascrivere file esistenti:
```shell
mv -i {{sorgente}} {{destinazione}}
```
#### Sposta file senza sovrascrivere file esistenti:
```shell
mv -n {{sorgente}} {{destinazione}}
```
#### Sposta file in modità verbosa, mostrando a schermo ogni file che viene spostato:
```shell
mv -v {{sorgente}} {{destinazione}}
```
{% endraw %}