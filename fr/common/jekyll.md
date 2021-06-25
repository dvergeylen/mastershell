---
layout: default
title: "jekyll"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jekyll">
  <a href="/fr/common/jekyll.html">jekyll</a> <a href="#jekyll"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Générateur de site statique simple, adapté aux blogs.
> Plus d'informations : <https://jekyllrb.com>.

#### Génère un serveur de développement qui tourne en http://localhost:4000/ :
```shell
jekyll serve
```
#### Active la régénération incrémentale :
```shell
jekyll serve --incremental
```
#### Active la sortie verbeuse :
```shell
jekyll serve --verbose
```
#### Génère le répertoire actuel dans `./_site` :
```shell
jekyll build
```
#### Nettoie le site (c.-à.-d. supprime la sortie du site et le répertoire `cache`) sans compiler :
```shell
jekyll clean
```
{% endraw %}