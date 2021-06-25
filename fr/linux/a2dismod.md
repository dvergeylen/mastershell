---
layout: default
title: "a2dismod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="a2dismod">
  <a href="/fr/linux/a2dismod.html">a2dismod</a> <a href="#a2dismod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Désactive un module Apache sur une distribution Debian.
> Plus d'informations : <https://manpages.debian.org/latest/apache2/a2dismod.8.en.html>.

#### Désactive un module :
```shell
sudo a2dismod {{module}}
```
#### N'affiche aucun message (mode silencieux) :
```shell
sudo a2dismod --quiet {{module}}
```
{% endraw %}