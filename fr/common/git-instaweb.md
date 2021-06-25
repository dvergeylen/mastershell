---
layout: default
title: "git instaweb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-instaweb">
  <a href="/fr/common/git-instaweb.html">git instaweb</a> <a href="#git-instaweb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Outil pour le lancement d'un serveur gitweb.
> Plus d'informations : <https://git-scm.com/docs/git-instaweb>.

#### Démarre un serveur gitweb depuis le dépôt (`repository`) courant :
```shell
git instaweb --start
```
#### Écoute uniquement sur le port localhost :
```shell
git instaweb --start --local
```
#### Écoute sur un port spécifique :
```shell
git instaweb --start --port {{1234}}
```
#### Utiliser un daemon http spécifique :
```shell
git instaweb --start --httpd {{lighttpd|apache2|mongoose|plackup|webrick}}
```
#### Lancer en même temps qu'un navigateur web :
```shell
git instaweb --start --browser
```
#### Stoppe le serveur :
```shell
git instaweb --stop
```
#### Redémarre le serveur :
```shell
git instaweb --restart
```
{% endraw %}