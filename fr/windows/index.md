---
layout: default
title: "windows"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#whoami">whoami</a>

{% raw %}
<h2 id="whoami">
  <a href="/fr/windows/whoami.html">whoami</a> <a href="#whoami"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Affiche des détails sur l'utilisateur courant.
> Plus d'informations : <https://docs.microsoft.com/windows-server/administration/windows-commands/whoami>.

#### Affiche le nom de l'utilisateur courant :
```shell
whoami
```
#### Affiche les groupes pour lesquels l'utilisateur courant est un membre :
```shell
whoami /groups
```
#### Affiche les droits de l'utilisateur courant :
```shell
whoami /priv
```
#### Affiche le nom principal d'utilisateur (UPN) de l'utilisateur courant :
```shell
whoami /upn
```
#### Affiche l'identifiant de connexion de l'utilisateur courant :
```shell
whoami /logonid
```
{% endraw %}