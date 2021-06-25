---
layout: default
title: "apt-add-repository"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-add-repository">
  <a href="/fr/linux/apt-add-repository.html">apt-add-repository</a> <a href="#apt-add-repository"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gère la définition des dépôts apt.
> Plus d'informations : <https://manpages.debian.org/latest/software-properties-common/apt-add-repository.1.html>.

#### Ajout d'un nouveau dépôt :
```shell
apt-add-repository {{repository_spec}}
```
#### Suppression d'un dépôt :
```shell
apt-add-repository --remove {{repository_spec}}
```
#### Mise à jour du cache des paquets après ajout d'un dépôt :
```shell
apt-add-repository --update {{repository_spec}}
```
#### Activation pour les paquets source :
```shell
apt-add-repository --enable-source {{repository_spec}}
```
{% endraw %}