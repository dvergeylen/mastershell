---
layout: default
title: "git rm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-rm">
  <a href="/fr/common/git-rm.html">git rm</a> <a href="#git-rm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Supprimer des fichiers de l'index, du dépôt et du système de fichiers.
> Plus d'informations : <https://git-scm.com/docs/git-rm>.

#### Supprimer un fichiers de l'index, du dépôt et du système de fichiers :
```shell
git rm {{file}}
```
#### Supprimer un répertoire de l'index, du dépôt et du système de fichiers :
```shell
git rm -r {{directory}}
```
#### Supprimer un fichiers de l'index, du dépôt mais le conserve sur le système de fichiers :
```shell
git rm --cached {{file}}
```
{% endraw %}