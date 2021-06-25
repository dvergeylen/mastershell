---
layout: default
title: "git commit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-commit">
  <a href="/it/common/git-commit.html">git commit</a> <a href="#git-commit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Salva file nell'area di stage in una nuova istantanea del tuo repository.
> Maggiori informazioni: <https://git-scm.com/docs/git-commit>.

#### Committa sul repository i file nell'area di stage con un messaggio:
```shell
git commit -m "{{messaggio}}"
```
#### Aggiungi all'area di stage tutti i file modificati e committali con un messaggio:
```shell
git commit -a -m "{{messaggio}}"
```
#### Sostituisci l'ultimo commit con le modifiche attualmente salvate nell'area di stage:
```shell
git commit --amend
```
#### Committa solo i file specificati (tra quelli presenti nell'area di stage):
```shell
git commit {{percorso/al/file1}} {{percorso/al/file2}}
```
{% endraw %}