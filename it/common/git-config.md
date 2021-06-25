---
layout: default
title: "git config"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-config">
  <a href="/it/common/git-config.html">git config</a> <a href="#git-config"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Configura le impostazioni di uno o piu repository Git.
> Le configurazioni possono essere sia locali (per il repository corrente) che globali (per l'utente corrente).
> Maggiori informazioni: <https://git-scm.com/docs/git-config>.

#### Elenca solo le opzioni di configurazione locali (salvate in `.git/config` nel repository corrente):
```shell
git config --list --local
```
#### Elenca solo le opzioni di configurazione globali (salvate in `~/.gitconfig`):
```shell
git config --list --global
```
#### Elenca tutte le opzioni di configurazione impostate, sia locali che globali:
```shell
git config --list
```
#### Mostra il valore di una data opzione di configurazione:
```shell
git config alias.unstage
```
#### Imposta il valore globale di una data opzione di configurazione:
```shell
git config --global alias.unstage "reset HEAD --"
```
#### Ripristina una opzione di configurazione globale al suo valore di default:
```shell
git config --global --unset alias.unstage
```
{% endraw %}