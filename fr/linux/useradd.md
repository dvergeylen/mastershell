---
layout: default
title: "useradd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="useradd">
  <a href="/fr/linux/useradd.html">useradd</a> <a href="#useradd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crée un nouvel utilisateur.
> Plus d'informations : <https://manned.org/useradd>.

#### Crée un nouvel utilisateur :
```shell
useradd {{nom}}
```
#### Crée un nouvel utilisateur avec un dossier home par défaut :
```shell
useradd --create-home {{nom}}
```
#### Crée un nouvel utilisateur avec le shell spécifié :
```shell
useradd --shell {{/chemin/vers/shell}} {{nom}}
```
#### Crée un nouvel utilisateur qui appartient aux groupes supplémentaires (attention à l'omission des espaces) :
```shell
useradd --groups {{groupe1,groupe2}} {{nom}}
```
#### Crée un nouvel utilisateur sans un dossier home :
```shell
useradd --no-create-home --system {{nom}}
```
{% endraw %}