---
layout: default
title: "git submodule"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-submodule">
  <a href="/it/common/git-submodule.html">git submodule</a> <a href="#git-submodule"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ispeziona, aggiorna e gestisce moduli secondari (submodule).
> Maggiori informazioni: <https://git-scm.com/docs/git-submodule>.

#### Installa specifici moduli secondari di un repository:
```shell
git submodule update --init --recursive
```
#### Aggiungi un repository Git come modulo secondario:
```shell
git submodule add {{url_repository}}
```
#### Aggiungi un repository Git come modulo secondario alla cartella specificata:
```shell
git submodule add {{url_repository}} {{percorso/alla/cartella}}
```
#### Aggiorna tutti i moduli secondari al loro commit più recente:
```shell
git submodule foreach git pull
```
{% endraw %}