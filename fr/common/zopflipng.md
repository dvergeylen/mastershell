---
layout: default
title: "zopflipng"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zopflipng">
  <a href="/fr/common/zopflipng.html">zopflipng</a> <a href="#zopflipng"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilitaire de compression d'images PNG.
> Plus d'informations : <https://github.com/google/zopfli>.

#### Optimise une image PNG :
```shell
zopflipng {{entrée.png}} {{sortie.png}}
```
#### Optimise plusieurs images PNG et sauvegarde avec préfixe donné :
```shell
zopflipng --prefix={{prefix}} {{image1.png}} {{image2.png}} {{image3.png}}
```
{% endraw %}