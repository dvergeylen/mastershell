---
layout: default
title: "borg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="borg">
  <a href="/fr/common/borg.html">borg</a> <a href="#borg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Outil de sauvegarde avec dé-duplication.
> Crée des sauvegardes distantes ou locales qui peuvent être montées comme un système de fichiers.
> Plus d'informations : <https://borgbackup.readthedocs.io/en/stable/usage/general.html>.

#### Initialise un dépôt local :
```shell
borg init {{/chemin/vers/repertoire_du_depot}}
```
#### Sauvegarde un répertoire dans le dépôt en créant une archive appelée "Lundi" :
```shell
borg create --progress {{/chemin/vers/repertoire_du_depot}}::{{Lundi}} {{/chemin/vers/repertoire_source}}
```
#### Liste toutes les archives d'un dépôt :
```shell
borg list {{/chemin/vers/repertoire_du_depot}}
```
#### Extrait un répertoire donné de l'archive nommée "Lundi" à partir d'un dépôt distant tout en excluant tous les fichiers *.ext :
```shell
borg extract {{utilisateur}}@{{hote}}:{{/chemin/vers/repertoire_du_depot}}::{{Lundi}} {{chemin/vers/repertoire_destination}} --exclude '{{*.ext}}'
```
#### Nettoie un dépôt en effaçant toutes les archives âgées de plus de 7 jours tout en affichant les changements :
```shell
borg prune --keep-within {{7d}} --list {{/chemin/vers/repertoire_du_depot}}
```
#### Monte un dépôt comme un système de fichiers FUSE :
```shell
borg mount {{/chemin/vers/repertoire_du_depot}}::{{Lundi}} {{/chemin/vers/point_de_montage}}
```
#### Affiche l'aide sur la création d'archives :
```shell
borg create --help
```
{% endraw %}