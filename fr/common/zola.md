---
layout: default
title: "zola"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zola">
  <a href="/fr/common/zola.html">zola</a> <a href="#zola"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un générateur de site statique à partir d'un unique binaire sans dépendance.
> Plus d'informations : <https://www.getzola.org/documentation/getting-started/cli-usage/>.

#### Créer la structure du répertoire utilisé par Zola dans un répertoire donné :
```shell
zola init {{mon_site}}
```
#### Construit la totalité du site dans le répertoire `public` (si le répertoire existe, il est supprimé) :
```shell
zola build
```
#### Construit la totalité du site dans un répertoire différent :
```shell
zola build --output-dir {{chemin/du/répertoire_de_sortie/}}
```
#### Construit et met à disposition le site à partir d'un serveur local (l'adresse par défaut est `127.0.0.1:1111`) :
```shell
zola serve
```
#### Construit l'ensemble des pages comme la commande `build`, sans écrire le résultat sur le disque :
```shell
zola check
```
{% endraw %}