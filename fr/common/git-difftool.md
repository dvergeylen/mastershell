---
layout: default
title: "git difftool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-difftool">
  <a href="/fr/common/git-difftool.html">git difftool</a> <a href="#git-difftool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Afficher les modifications apportées aux fichiers à l'aide d'outils de comparaison externes. Accepte les mêmes options et arguments que Git diff.
> Plus d'informations : <https://git-scm.com/docs/git-difftool>.

#### Lister les outils de comparaison disponibles :
```shell
git difftool --tool-help
```
#### Configurer Meld comme outil de comparaison par défaut :
```shell
git config --global diff.tool "{{meld}}"
```
#### Utiliser l'outil de comparaison par défaut pour afficher les fichiers modifiés :
```shell
git difftool --staged
```
#### Utiliser un outil de comparaison spécifique (opendiff) pour afficher les changements depuis un commit :
```shell
git difftool --tool={{opendiff}} {{commit}}
```
{% endraw %}