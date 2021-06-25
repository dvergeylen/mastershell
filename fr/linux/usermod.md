---
layout: default
title: "usermod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="usermod">
  <a href="/fr/linux/usermod.html">usermod</a> <a href="#usermod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Modifie un compte utilisateur.
> Plus d'informations : <https://manned.org/usermod>.

#### Change le nom d'un utilisateur :
```shell
usermod -l {{nouveau_nom}} {{utilisateur}}
```
#### Ajoute l'utilisateur à des groupes supplémentaires (attention à l'omission d'espaces) :
```shell
usermod -a -G {{groupe1,groupe2}} {{utilisateur}}
```
#### Crée un nouveau dossier home pour un utilisateur et déplace ses fichiers vers celui-ci :
```shell
usermod -m -d {{/chemin/vers/home}} {{utilisateur}}
```
{% endraw %}