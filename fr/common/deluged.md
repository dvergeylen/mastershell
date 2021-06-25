---
layout: default
title: "deluged"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="deluged">
  <a href="/fr/common/deluged.html">deluged</a> <a href="#deluged"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un processus démon pour le client BitTorrent Deluge.
> Plus d'informations : <https://deluge-torrent.org>.

#### Lance le démon Deluge :
```shell
deluged
```
#### Lance le démon Deluge sur un port spécifique :
```shell
deluged -p {{port}}
```
#### Lance le démon Deluge à l'aide d'un fichier de configuration spécifique :
```shell
deluged -c {{chemin/vers/fichier_configuration}}
```
#### Lance le démon Deluge et enregistre les journaux dans un fichier :
```shell
deluged -l {{chemin/vers/fichier_journalisation}}
```
{% endraw %}