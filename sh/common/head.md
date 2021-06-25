---
layout: default
title: "head"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="head">
  <a href="/sh/common/head.html">head</a> <a href="#head"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Prikazuje prvi deo datoteka.
> Više informacija: <https://www.gnu.org/software/coreutils/head>.

#### Prikaži prvih nekoliko linija datoteke:
```shell
head -n {{broj_linija}} {{naziv_datoteke}}
```
#### Prikaži prvih nekoliko bajtova datoteke:
```shell
head -c {{veličina_u_bajtovima}} {{naziv_datoteke}}
```
#### Prikaži sve osim nekoliko poslednjih linija datoteke:
```shell
head -n -{{broj_linija}} {{naziv_datoteke}}
```
#### Prikaži sve osim nekoliko poslednjih bajtova datoteke:
```shell
head -c -{{veličina_u_bajtovima}} {{naziv_datoteke}}
```
{% endraw %}