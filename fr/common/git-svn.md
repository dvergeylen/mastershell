---
layout: default
title: "git svn"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-svn">
  <a href="/fr/common/git-svn.html">git svn</a> <a href="#git-svn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Opération bidirectionnelle entre un référentiel Subversion et Git.
> Plus d'informations : <https://git-scm.com/docs/git-svn>.

#### Cloner un dépôt SVN :
```shell
git svn clone {{https://example.com/subversion_repo}} {{local_dir}}
```
#### Cloner un dépôt SVN à partir d'une révision donnée :
```shell
git svn clone -r{{1234}}:HEAD {{https://svn.example.net/subversion/repo}} {{local_dir}}
```
#### Mettre à jour le clone local à partir du dépôt SVN distant :
```shell
git svn rebase
```
#### Chercher les changements distants dans le dépôt SVN dans les appliquer sur le HEAD :
```shell
git svn fetch
```
#### Commiter sur le SVN :
```shell
git svn commit
```
{% endraw %}