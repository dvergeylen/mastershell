---
layout: default
title: "ifdown"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ifdown">
  <a href="/fr/linux/ifdown.html">ifdown</a> <a href="#ifdown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Désactive des interfaces réseau.
> Plus d'informations : <https://manned.org/ifdown>.

#### Désactive l'interface eth0 :
```shell
ifdown {{eth0}}
```
#### Désactive toutes les interfaces déjà actives :
```shell
ifdown -a
```
{% endraw %}