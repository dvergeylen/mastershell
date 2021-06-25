---
layout: default
title: "git bundle"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-bundle">
  <a href="/it/common/git-bundle.html">git bundle</a> <a href="#git-bundle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Colloca oggetti e riferimenti in un archivio.
> Maggiori informazioni: <https://git-scm.com/docs/git-bundle>.

#### Crea un file bundle che contiene tutti gli oggetti e riferimenti di un dato ramo:
```shell
git bundle create {{percorso/al/file.bundle}} {{nome_ramo}}
```
#### Crea un file bundle di tutti i rami:
```shell
git bundle create {{percorso/al/file.bundle}} --all
```
#### Crea un file bundle degli ultimi 5 commit sul ramo corrente:
```shell
git bundle create {{percorso/al/file.bundle}} -{{5}} {{HEAD}}
```
#### Crea un file bundle degli ultimi 7 giorni:
```shell
git bundle create {{percorso/al/file.bundle}} --since={{7.days}} {{HEAD}}
```
#### Verifica che un file bundle sia valido e possa essere applicato al repository in uso:
```shell
git bundle verify {{percorso/al/file.bundle}}
```
#### Stampa su standard output la lista di riferimenti contenuti in un bundle:
```shell
git bundle unbundle {{percorso/al/file.bundle}}
```
#### Dato un file bundle, estrai un ramo specifico nel repository in uso:
```shell
git pull {{percorso/al/file.bundle}} {{nome_ramo}}
```
{% endraw %}