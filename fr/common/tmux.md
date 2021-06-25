---
layout: default
title: "tmux"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tmux">
  <a href="/fr/common/tmux.html">tmux</a> <a href="#tmux"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Multiplexeur de terminaux. Permet plusieurs sessions avec fenêtres, panneaux, et plus encore.
> Plus d'informations : <https://github.com/tmux/tmux>.

#### Démarrer une nouvelle session :
```shell
tmux
```
#### Démarrer une nouvelle session nommée :
```shell
tmux new-session -s {{nom}}
```
#### Lister les sessions existantes :
```shell
tmux ls
```
#### S'attacher à la session utilisée la plus récemment :
```shell
tmux attach-session
```
#### S'attacher à une session nommée :
```shell
tmux attach-session -t {{nom}}
```
#### Se détacher de la session actuelle (avec le préfixe Ctrl-B) :
```shell
Ctrl-B d
```
#### Détruire une session nommée :
```shell
tmux kill-session -t {{nom}}
```
#### Détruire la session actuelle (avec le préfixe Ctrl-B) :
```shell
Ctrl-B :kill-session<Enter>
```
{% endraw %}