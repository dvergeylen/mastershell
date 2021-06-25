---
layout: default
title: "a2enconf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="a2enconf">
  <a href="/fr/linux/a2enconf.html">a2enconf</a> <a href="#a2enconf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Active un fichier de configuration sur une distribution Debian.
> Plus d'information : <https://manpages.debian.org/latest/apache2/a2enconf.8.en.html>.

#### Active un fichier de configuration :
```shell
sudo a2enconf {{fichier_de_configuration}}
```
#### N'affiche aucun message (mode silencieux) :
```shell
sudo a2enconf --quiet {{fichier_de_configuration}}
```
{% endraw %}