---
layout: default
title: "a2dissite"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="a2dissite">
  <a href="/fr/linux/a2dissite.html">a2dissite</a> <a href="#a2dissite"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Désactive un hôte virtuel Apache sur une distribution Debian.
> Plus d'informations : <https://manpages.debian.org/latest/apache2/a2dissite.8.en.html>.

#### Désactive un hôte virtuel :
```shell
sudo a2dissite {{virtual_host}}
```
#### N'affiche aucun message (mode silencieux) :
```shell
sudo a2dissite --quiet {{virtual_host}}
```
{% endraw %}