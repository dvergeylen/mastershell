---
layout: default
title: "git switch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-switch">
  <a href="/it/common/git-switch.html">git switch</a> <a href="#git-switch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Passa ad altri rami. Richiede versioni di Git successive alla 2.23.
> Vedi anche `git checkout`.
> Maggiori informazioni: <https://git-scm.com/docs/git-switch>.

#### Passa ad un altro ramo esistente:
```shell
git switch {{nome_ramo}}
```
#### Crea un nuovo ramo e passa a quel ramo:
```shell
git switch --create {{nome_ramo}}
```
#### Crea un nuovo ramo a partire da un commit esistente e passa a quel ramo:
```shell
git switch --create {{nome_ramo}} {{commit}}
```
#### Torna al ramo precedente:
```shell
git switch -
```
#### Passa ad un ramo ed aggiorna tutti i moduli secondari associati:
```shell
git switch --recurse-submodules {{nome_ramo}}
```
#### Passa ad un ramo e uniscilo automaticamente al ramo corrente, include le modifiche non committate:
```shell
git switch --merge {{nome_ramo}}
```
{% endraw %}