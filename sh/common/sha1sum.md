---
layout: default
title: "sha1sum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sha1sum">
  <a href="/sh/common/sha1sum.html">sha1sum</a> <a href="#sha1sum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Izračunava SHA1 kriptografske kontrolne brojeve.
> Više informacija: <https://www.gnu.org/software/coreutils/sha1sum>.

#### Izračunaj SHA1 kontrolni broj za datoteku:
```shell
sha1sum {{datoteka1}}
```
#### Izračunaj SHA1 kontrolne brojeve za više datoteka:
```shell
sha1sum {{datoteka1}} {{datoteka2}}
```
#### Pročitaj datoteku SHA1 brojeva i proveri da li se svi kontrolni brojevi datoteka poklapaju:
```shell
sha1sum -c {{datoteka.sha1}}
```
{% endraw %}