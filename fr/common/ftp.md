---
layout: default
title: "ftp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ftp">
  <a href="/fr/common/ftp.html">ftp</a> <a href="#ftp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Outils permettant d'interagir avec un serveur avec le protocole FTP.

#### Se connecter à un serveur FTP :
```shell
ftp {{ftp.exemple.com}}
```
#### Passer au mode de transfert binaire (médias, fichiers compressés, etc) :
```shell
binary
```
#### Transférer plusieurs fichiers sans demander de confirmation pour chaque :
```shell
prompt off
```
#### Télécharger plusieurs fichiers :
```shell
mget {{*.png}}
```
#### Uploader plusieurs fichiers :
```shell
mput {{*.zip}}
```
#### Supprimer plusieurs fichiers sur le serveur distant :
```shell
mdelete {{*.txt}}
```
#### Renommer un fichier sur le serveur distant :
```shell
rename {{ancien_fichier}} {{nouveau_fichier}}
```
{% endraw %}