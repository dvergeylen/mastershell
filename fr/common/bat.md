---
layout: default
title: "bat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bat">
  <a href="/fr/common/bat.html">bat</a> <a href="#bat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Affiche et concatène le contenu d'un ou plusieurs fichiers.
> Un clone de `cat` avec mise en valeur de la syntaxe et intégration avec Git.
> Plus d'informations : <https://github.com/sharkdp/bat>.

#### Affiche le contenu d'un fichier sur la sortie standard :
```shell
bat {{fichier}}
```
#### Concatène le contenu de plusieurs fichiers vers le fichier de destination :
```shell
bat {{fichier1}} {{fichier2}} > {{fichier_de_destination}}
```
#### Ajoute le contenu d'un ficher à la fin du fichier de destination :
```shell
bat {{fichier1}} {{fichier2}} >> {{fichier_de_destination}}
```
#### Numérote toutes les lignes affichées :
```shell
bat -n {{fichier}}
```
#### Affiche le contenu d'un fichier JSON sur la sortie standard avec mise en valeur de la syntaxe :
```shell
bat --language json {{fichier.json}}
```
#### Affiche tous les langages pris en charge :
```shell
bat --list-languages
```
{% endraw %}