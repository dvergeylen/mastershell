---
layout: default
title: "cp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cp">
  <a href="/it/common/cp.html">cp</a> <a href="#cp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copia file e directory.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/cp>.

#### Copia un file in un'altra posizione:
```shell
cp {{percorso/al/file}} {{percorso/alla/copia}}
```
#### Copia un file in una directory mantenendo il nome:
```shell
cp {{percorso/al/file}} {{percorso/alla/directory}}
```
#### Copia una directory ricorsivamente in un'altra posizione:
```shell
cp -r {{percorso/alla/directory}} {{percorso/alla/copia}}
```
#### Copia una directory ricorsivamente in modo verboso (mostra a schermo ogni file copiato):
```shell
cp -vr {{percorso/alla/directory}} {{percorso/alla/copia}}
```
#### Copia i contenuti di una directory in una seconda directory:
```shell
cp -r {{percorso/alla/directory/*}} {{percorso/alla/seconda/directory}}
```
#### Copia tutti i file di testo in una seconda directory in modo interattivo (chiede conferma prima di sovrascrivere):
```shell
cp -i {{*.txt}} {{percorso/alla/directory}}
```
{% endraw %}