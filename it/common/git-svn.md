---
layout: default
title: "git svn"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-svn">
  <a href="/it/common/git-svn.html">git svn</a> <a href="#git-svn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Operazioni bidirezionali tra repository Subversion e Git.
> Maggiori informazioni: <https://git-scm.com/docs/git-svn>.

#### Clona un repository SVN:
```shell
git svn clone {{https://esempio.com/repo_subversion}} {{cartella_locale}}
```
#### Clona un repository SVN a partire da uno specifico numero di revisione:
```shell
git svn clone -r{{1234}}:HEAD {{https://svn.esempio.net/subversion/repo}} {{cartella_locale}}
```
#### Aggiorna una copia locale da un repository SVN remoto:
```shell
git svn rebase
```
#### Scarica aggiornamenti da un repository SVN remoto senza spostare l'HEAD Git:
```shell
git svn fetch
```
#### Invia un commit a un repository SVN:
```shell
git svn dcommit
```
{% endraw %}