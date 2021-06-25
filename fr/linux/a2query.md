---
layout: default
title: "a2query"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="a2query">
  <a href="/fr/linux/a2query.html">a2query</a> <a href="#a2query"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Retourne la configuration d'exécution d'Apache sur une distribution Debian.
> Plus d'informations : <https://manpages.debian.org/latest/apache2/a2query.1.en.html>.

#### Liste les [m]odules Apache actifs :
```shell
sudo a2query -m
```
#### Vérifie si un module spécifique est installé :
```shell
sudo a2query -m {{nom_module}}
```
#### Liste les hôtes virtuels actifs :
```shell
sudo a2query -s
```
#### Affiche le [M]odule de traitement multiple actif :
```shell
sudo a2query -M
```
#### Affiche la [v]ersion d'Apache :
```shell
sudo a2query -v
```
{% endraw %}