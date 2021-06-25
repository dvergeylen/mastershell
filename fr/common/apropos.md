---
layout: default
title: "apropos"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apropos">
  <a href="/fr/common/apropos.html">apropos</a> <a href="#apropos"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Recherche dans les pages de manuel, par exemple pour trouver une nouvelle commande.
> Plus d'informations : <https://manned.org/apropos>.

#### Recherche par mot clé :
```shell
apropos {{expression_reguliere}}
```
#### Recherche sans limiter la sortie à la largeur du terminal :
```shell
apropos -l {{expression_reguliere}}
```
#### Recherche les pages qui contiennent toutes les expressions données (fonction ET) :
```shell
apropos {{expression_reguliere_1}} -a {{expression_reguliere_2}} -a {{expression_reguliere_3}}
```
{% endraw %}