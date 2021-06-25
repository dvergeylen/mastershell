---
layout: default
title: "atom"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="atom">
  <a href="/fr/common/atom.html">atom</a> <a href="#atom"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un éditeur de texte multiplateforme proposant de nombreuses extensions.
> Les extensions sont gérées par `apm`.
> Plus d'informations : <https://atom.io/>.

#### Ouvrir un fichier ou un dossier :
```shell
atom {{chemin/vers/fichier_ou_dossier}}
```
#### Ouvrir un fichier ou un dossier dans une nouvelle fenêtre :
```shell
atom -n {{chemin/vers/fichier_ou_dossier}}
```
#### Ouvrir un fichier ou un dossier dans une fenêtre existante :
```shell
atom --add {{chemin/vers/fichier_ou_dossier}}
```
#### Ouvrir en mode sans-échec (les extensions ne seront pas chargées) :
```shell
atom --safe
```
#### Empêcher Atom de se lancer en arrière-plan, en le forçant à s'attacher au terminal :
```shell
atom --foreground
```
#### Attendre la fermeture de la fenêtre avant de quitter (utile pour l'éditeur de commits Git) :
```shell
atom --wait
```
{% endraw %}