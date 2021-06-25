---
layout: default
title: "git stage"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-stage">
  <a href="/it/common/git-stage.html">git stage</a> <a href="#git-stage"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Aggiungi file all'area di stage.
> Sinonimo di `git add`.
> Maggiori informazioni: <https://git-scm.com/docs/git-stage>.

#### Aggiungi un file all'indice:
```shell
git stage {{percorso/al/file}}
```
#### Aggiungi tutti i file (tracciati e non):
```shell
git stage -A
```
#### Aggiungi solo file già tracciati:
```shell
git stage -u
```
#### Aggiungi anche file ignorati:
```shell
git stage -f
```
#### Aggiungi parti di file all'area di stage in modo interattivo:
```shell
git stage -p
```
#### Aggiungi parti di un dato file all'area di stage in modo interattivo:
```shell
git stage -p {{percorso/al/file}}
```
#### Aggiungi all'area di stage in modo interattivo:
```shell
git stage -i
```
{% endraw %}