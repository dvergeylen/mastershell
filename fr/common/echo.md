---
layout: default
title: "echo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="echo">
  <a href="/fr/common/echo.html">echo</a> <a href="#echo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Affiche les paramètres donnés dans la console.
> Plus d'informations : <https://www.gnu.org/software/coreutils/echo>.

#### Affiche un message (les guillemets sont facultatifs) :
```shell
echo "{{Hello World}}"
```
#### Affiche un message avec des variables d'environnement :
```shell
echo "{{Ma variable PATH est $PATH}}"
```
#### Affiche un message sans retour à la ligne :
```shell
echo -n "{{Hello World}}"
```
#### Ajoute un message à un fichier :
```shell
echo "{{Hello World}}" >> {{fichier.txt}}
```
#### Active l'interprétation des spécificateurs d'échappement :
```shell
echo -e "{{Colonne 1\tColonne 2}}"
```
{% endraw %}