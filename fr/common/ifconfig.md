---
layout: default
title: "ifconfig"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ifconfig">
  <a href="/fr/common/ifconfig.html">ifconfig</a> <a href="#ifconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Configurateur des interfaces réseau.

#### Affiche les paramètres de réseau d'un adaptateur ethernet :
```shell
ifconfig {{eth0}}
```
#### Affiche les détails de toutes les interfaces, y compris les interfaces désactivées :
```shell
ifconfig -a
```
#### Désactive l'interface eth0 :
```shell
ifconfig {{eth0}} down
```
#### Active l'interface eth0 :
```shell
ifconfig {{eth0}} up
```
#### Assigne une adresse IP à l'interface eth0 :
```shell
ifconfig {{eth0}} {{addresse_ip}}
```
{% endraw %}