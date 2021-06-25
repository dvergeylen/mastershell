---
layout: default
title: "git mergetool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-mergetool">
  <a href="/fr/common/git-mergetool.html">git mergetool</a> <a href="#git-mergetool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Executer un utilitaire de différences pour résoudre les conflits de merge.
> Plus d'informations : <https://git-scm.com/docs/git-mergetool>.

#### Démarrer l'outil de différences par défaut :
```shell
git mergetool
```
#### Lister les outils de différences valides :
```shell
git mergetool --tool-help
```
#### Démarrer l'outil de différences en précisant son nom :
```shell
git mergetool --tool {{tool_name}}
```
#### Démarrer l'outil de différences sans dialogues :
```shell
git mergetool --no-prompt
```
#### Utiliser explicitement l'outil de différences graphique (voir la variable de config `merge.guitool`) :
```shell
git mergetool --gui
```
#### Utiliser explicitement l'outil de différences classique (voir la variable de config `merge.tool`) :
```shell
git mergetool --no-gui
```
{% endraw %}