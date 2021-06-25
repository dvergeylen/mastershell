---
layout: default
title: "deluge"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="deluge">
  <a href="/fr/common/deluge.html">deluge</a> <a href="#deluge"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Client BitTorrent à base de ligne de commande.
> Plus d'informations : <https://deluge-torrent.org>.

#### Télécharge un torrent :
```shell
deluge {{url|magnet|chemin/vers/fichier}}
```
#### Télécharge un torrent à l'aide d'un fichier de configuration particulier :
```shell
deluge -c {{chemin/vers/fichier_configuration}} {{url|magnet|chemin/vers/fichier}}
```
#### Télécharge un torrent et lance un interface usager particulier :
```shell
deluge -u {{gtk|web|console}} {{url|magnet|chemin/vers/fichier}}
```
#### Télécharge un torrent et enregistre les journaux dans un ficher :
```shell
deluge -l {{chemin/vers/fichier_journalisation}} {{url|magnet|chemin/vers/fichier}}
```
{% endraw %}