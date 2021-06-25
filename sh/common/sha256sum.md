---
layout: default
title: "sha256sum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sha256sum">
  <a href="/sh/common/sha256sum.html">sha256sum</a> <a href="#sha256sum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Izračunava SHA256 kriptografske kontrolne brojeve.
> Više informacija: <https://www.gnu.org/software/coreutils/manual/html_node/sha2-utilities.html>.

#### Izračunaj SHA256 kontrolni broj za datoteku:
```shell
sha256sum {{datoteka1}}
```
#### Izračunaj SHA256 kontrolne brojeve za više datoteka:
```shell
sha256sum {{datoteka1}} {{datoteka2}}
```
#### Pročitaj datoteku SHA256 brojeva i proveri da li se svi kontrolni brojevi datoteka poklapaju:
```shell
sha256sum -c {{datoteka.sha256}}
```
{% endraw %}