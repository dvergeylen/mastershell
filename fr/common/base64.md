---
layout: default
title: "base64"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="base64">
  <a href="/fr/common/base64.html">base64</a> <a href="#base64"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Encoder ou décoder un fichier ou l'entrée standard en utilisant le codage Base64 à destination de la sortie standard.
> Plus d'informations : <https://www.gnu.org/software/coreutils/base64>.

#### Encoder un fichier :
```shell
base64 {{fichier}}
```
#### Décoder un fichier :
```shell
base64 --decode {{fichier}}
```
#### Encoder depuis stdin :
```shell
{{une_commande}} | base64
```
#### Décoder depuis stdin :
```shell
{{une_commande}} | base64 --decode
```
{% endraw %}