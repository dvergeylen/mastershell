---
layout: default
title: "git lfs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-lfs">
  <a href="/fr/common/git-lfs.html">git lfs</a> <a href="#git-lfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Travailler dans un registre Git avec des fichiers volumineux.
> Plus d'informations : <https://git-lfs.github.com>.

#### Initialise le Git LFS :
```shell
git lfs install
```
#### Suivre des fichiers correspondant à un pattern :
```shell
git lfs track '{{*.bin}}'
```
#### Changer l'URL du point de terminaison Git LFS (utile si le serveur LFS est séparé du serveur Git) :
```shell
git config -f .lfsconfig lfs.url {{lfs_endpoint_url}}
```
#### Lister les pattern de fichiers suivis :
```shell
git lfs track
```
#### Lister les fichiers suivis ayant été commité :
```shell
git lfs ls-files
```
#### Pousser tout les objets LFS vers le serveur distant :
```shell
git lfs push --all {{nom_distant}} {{nom_de_branche}}
```
#### Chercher tout les objets LFS :
```shell
git lfs fetch
```
#### Charger tout les objets LFS :
```shell
git lfs checkout
```
{% endraw %}