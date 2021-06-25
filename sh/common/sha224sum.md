---
layout: default
title: "sha224sum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sha224sum">
  <a href="/sh/common/sha224sum.html">sha224sum</a> <a href="#sha224sum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Izračunava SHA224 kriptografske kontrolne brojeve.
> Više informacija: <https://www.gnu.org/software/coreutils/manual/html_node/sha2-utilities.html>.

#### Izračunaj SHA224 kontrolni broj za datoteku:
```shell
sha224sum {{datoteka1}}
```
#### Izračunaj SHA224 kontrolne brojeve za više datoteka:
```shell
sha224sum {{datoteka1}} {{datoteka2}}
```
#### Pročitaj datoteku SHA224 brojeva i proveri da li se svi kontrolni brojevi datoteka poklapaju:
```shell
sha224sum -c {{datoteka.sha224}}
```
{% endraw %}