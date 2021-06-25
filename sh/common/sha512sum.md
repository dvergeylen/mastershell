---
layout: default
title: "sha512sum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sha512sum">
  <a href="/sh/common/sha512sum.html">sha512sum</a> <a href="#sha512sum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Izračunava SHA512 kriptografske kontrolne brojeve.
> Više informacija: <https://www.gnu.org/software/coreutils/manual/html_node/sha2-utilities.html>.

#### Izračunaj SHA512 kontrolni broj za datoteku:
```shell
sha512sum {{datoteka1}}
```
#### Izračunaj SHA512 kontrolne brojeve za više datoteka:
```shell
sha512sum {{datoteka1}} {{datoteka2}}
```
#### Pročitaj datoteku SHA512 brojeva i proveri da li se svi kontrolni brojevi datoteka poklapaju:
```shell
sha512sum -c {{datoteka.sha512}}
```
{% endraw %}