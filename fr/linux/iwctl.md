---
layout: default
title: "iwctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="iwctl">
  <a href="/fr/linux/iwctl.html">iwctl</a> <a href="#iwctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un outil de ligne de commande pour gérer iwd.
> Plus d'informations : <https://iwd.wiki.kernel.org/gettingstarted>.

#### Lancer le mode interactif, dans ce mode vous pouvez entrer les commandes directement, avec de l'auto-complétion :
```shell
iwctl
```
#### Avoir l'aide générale :
```shell
iwctl --help
```
#### Afficher vos stations wifi :
```shell
iwctl station list
```
#### Lancer la recherche de réseaux avec une station :
```shell
iwctl station {{station}} scan
```
#### Afficher les réseaux trouvés par une station :
```shell
iwctl station {{station}} get-networks
```
#### Se connecter à un réseau avec une station, si des informations de connexion sont nécessaires elles seront demandées :
```shell
iwctl station {{station}} connect {{nom_du_réseau}}
```
{% endraw %}