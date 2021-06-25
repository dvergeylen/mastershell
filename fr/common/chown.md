---
layout: default
title: "chown"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chown">
  <a href="/fr/common/chown.html">chown</a> <a href="#chown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Modifie l'utilisateur et le groupe propriétaire des fichiers et dossiers.
> Plus d'informations : <https://www.gnu.org/software/coreutils/chown>.

#### Modifie le propriétaire d'un fichier/dossier :
```shell
chown {{utilisateur}} {{chemin/vers/fichier_ou_dossier}}
```
#### Modifie l'utilisateur et le groupe propriétaire d'un fichier/dossier :
```shell
chown {{utilisateur}}:{{groupe}} {{chemin/vers/fichier_ou_dossier}}
```
#### Modifie récursivement le propriétaire d'un dossier et de son contenu :
```shell
chown -R {{utilisateur}} {{chemin/vers/dossier}}
```
#### Modifie le propriétaire d'un lien symbolique :
```shell
chown -h {{utilisateur}} {{chemin/vers/lien_symbolique}}
```
#### Modifie le propriétaire d'un fichier / dossier pour correspondre à un fichier de référence :
```shell
chown --reference={{chemin/vers/fichier_de_référence}} {{chemin/vers/fichier_ou_dossier}}
```
{% endraw %}