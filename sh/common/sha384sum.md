---
layout: default
title: "sha384sum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sha384sum">
  <a href="/sh/common/sha384sum.html">sha384sum</a> <a href="#sha384sum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Izračunava SHA384 kriptografske kontrolne brojeve.
> Više informacija: <https://www.gnu.org/software/coreutils/manual/html_node/sha2-utilities.html>.

#### Izračunaj SHA384 kontrolni broj za datoteku:
```shell
sha384sum {{datoteka1}}
```
#### Izračunaj SHA384 kontrolne brojeve za više datoteka:
```shell
sha384sum {{datoteka1}} {{datoteka2}}
```
#### Pročitaj datoteku SHA384 brojeva i proveri da li se svi kontrolni brojevi datoteka poklapaju:
```shell
sha384sum -c {{datoteka.sha384}}
```
{% endraw %}