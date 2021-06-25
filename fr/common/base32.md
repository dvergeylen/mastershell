---
layout: default
title: "base32"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="base32">
  <a href="/fr/common/base32.html">base32</a> <a href="#base32"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Encode ou décode un fichier ou l'entrée standard vers ou depuis la base 32, et retourne le résultat à la sortie standard.
> Plus d'informations : <https://www.gnu.org/software/coreutils/base32>.

#### Encode un fichier :
```shell
base32 {{fichier}}
```
#### Décode un fichier :
```shell
base32 --decode {{fichier}}
```
#### Encode depuis stdin :
```shell
{{commande}} | base32
```
#### Décode depuis stdin :
```shell
{{commande}} | base32 --decode
```
{% endraw %}