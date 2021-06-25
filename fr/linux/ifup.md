---
layout: default
title: "ifup"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ifup">
  <a href="/fr/linux/ifup.html">ifup</a> <a href="#ifup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Outil utilisé pour activer des interfaces réseau.
> Plus d'informations : <https://manpages.debian.org/latest/ifupdown/ifup.8.html>.

#### Active l'interface eth0 :
```shell
ifup {{eth0}}
```
#### Active l'ensemble des interfaces réseau définies dans le fichier `/etc/network/interfaces` :
```shell
ifup -a
```
{% endraw %}