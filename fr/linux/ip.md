---
layout: default
title: "ip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ip">
  <a href="/fr/linux/ip.html">ip</a> <a href="#ip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Affiche / manipule l'adressage, le routage, les interfaces et périphériques réseau, les règles de routage et les tunnels.
> Plus d'informations : <https://www.man7.org/linux/man-pages/man8/ip.8.html>.

#### Liste les interfaces avec des infos détaillées :
```shell
ip address
```
#### Liste les interfaces sur la couche réseau de façon synthétique :
```shell
ip -brief address
```
#### Liste les interfaces sur la couche liaison de façon synthétique :
```shell
ip -brief link
```
#### Affiche la table de routage :
```shell
ip route
```
#### Affiche les voisins (table ARP) :
```shell
ip neighbour
```
#### Active/Désactive une interface :
```shell
ip link set {{interface}} up/down
```
#### Ajoute/Supprime une adresse ip à une interface :
```shell
ip addr add/del {{ip}}/{{mask}} dev {{interface}}
```
#### Ajoute une route par défaut :
```shell
ip route add default via {{ip}} dev {{interface}}
```
{% endraw %}