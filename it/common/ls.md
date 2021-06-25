---
layout: default
title: "ls"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ls">
  <a href="/it/common/ls.html">ls</a> <a href="#ls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Elenca i contenuti di una directory.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/ls>.

#### Elenca i file nella directory corrente, uno per riga:
```shell
ls -1
```
#### Elenca tutti i file, inclusi quelli nascosti:
```shell
ls -a
```
#### Elenca tutti i file e mostra informazioni (permessi, dimensione e data di ultima modifica):
```shell
ls -la
```
#### Elenca tutti i file e mostra informazioni usando un formato facilmente leggibile (KiB, MiB, GiB):
```shell
ls -lh
```
#### Elenca tutti i file e mostra informazioni, ordinandoli per dimensione decrescente:
```shell
ls -lS
```
#### Elenca tutti i file e mostra informazioni, ordinandoli per ultima modifica:
```shell
ls -ltr
```
{% endraw %}