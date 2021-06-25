---
layout: default
title: "git"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git">
  <a href="/fr/common/git.html">git</a> <a href="#git"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Système de gestion de versions décentralisé.
> Plus d'informations : <https://git-scm.com/>.

#### Obtenir la version de Git :
```shell
git --version
```
#### Afficher l'aide générale :
```shell
git --help
```
#### Afficher l'aide sur une sous-commande Git :
```shell
git help {{sous_commande}}
```
#### Exécuter une sous-commande Git :
```shell
git {{sous_commande}}
```
#### Exécuter une sous-commande Git sur un répertoire personnalisé :
```shell
git -C {{chemin/vers/repertoire}} {{sous_commande}}
```
#### Exécuter une sous-commande Git avec un paramètre de configuration spécifique :
```shell
git -c '{{cle_param_config}}={{valeur}}' {{sous_commande}}
```
{% endraw %}