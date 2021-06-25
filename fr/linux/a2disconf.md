---
layout: default
title: "a2disconf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="a2disconf">
  <a href="/fr/linux/a2disconf.html">a2disconf</a> <a href="#a2disconf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Désactive un fichier de configuration sur une distribution Debian.
> Plus d'informations : <https://manpages.debian.org/latest/apache2/a2disconf.8.en.html>.

#### Désactive un fichier de configuration :
```shell
sudo a2disconf {{fichier_de_configuration}}
```
#### N'affiche aucun message (mode silencieux) :
```shell
sudo a2disconf --quiet {{fichier_de_configuration}}
```
{% endraw %}