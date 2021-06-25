---
layout: default
title: "ip address"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ip-address">
  <a href="/fr/linux/ip-address.html">ip address</a> <a href="#ip-address"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sous-commande de gestion des adresses IP.
> Plus d'informations : <https://www.man7.org/linux/man-pages/man8/ip-address.8.html>.

#### Liste les interfaces réseau et leurs adresses IP associées :
```shell
ip address
```
#### Filtre pour n'afficher que les interfaces réseau actives :
```shell
ip address show up
```
#### Affiche les informations relatives à une interface réseau spécifique :
```shell
ip address show dev {{eth0}}
```
#### Ajoute une adresse IP à une interface réseau :
```shell
ip address add {{ip_address}} dev {{eth0}}
```
#### Supprimer une adresse réseau d'une interface réseau :
```shell
ip address delete {{ip_address}} dev {{eth0}}
```
#### Supprime l'ensemble des adresses IP sur une portée donnée (scope) depuis une interface réseau :
```shell
ip address flush dev {{eth0}} scope {{global|host|link}}
```
{% endraw %}