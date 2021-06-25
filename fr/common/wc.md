---
layout: default
title: "wc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wc">
  <a href="/fr/common/wc.html">wc</a> <a href="#wc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compte les lignes, les mots ou les octets.
> Plus d'informations : <https://www.gnu.org/software/coreutils/wc>.

#### Compte les lignes d'un fichier :
```shell
wc -l {{file}}
```
#### Compte les mots d'un fichier :
```shell
wc -w {{file}}
```
#### Compte les caractères (octets) d'un fichier :
```shell
wc -c {{file}}
```
#### Compte les caractères d'un fichier (en prenant en compte l'ensemble des caractères multi-octets) :
```shell
wc -m {{file}}
```
{% endraw %}