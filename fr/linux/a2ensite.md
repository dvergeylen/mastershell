---
layout: default
title: "a2ensite"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="a2ensite">
  <a href="/fr/linux/a2ensite.html">a2ensite</a> <a href="#a2ensite"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Active un hôte virtuel Apache sur des systèmes d'exploitation (SE) basés sur Debian.
> Plus d'informations : <https://manpages.debian.org/latest/apache2/a2ensite.8.en.html>.

#### Active un hôte virtuel :
```shell
sudo a2ensite {{hote_virtuel}}
```
#### N'affiche aucun message (mode silencieux) :
```shell
sudo a2ensite --quiet {{hote_virtuel}}
```
{% endraw %}