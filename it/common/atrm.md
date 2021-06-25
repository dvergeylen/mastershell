---
layout: default
title: "atrm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="atrm">
  <a href="/it/common/atrm.html">atrm</a> <a href="#atrm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rimuovi job programmati dai comandi `at` o `batch`.
> Per trovare i numeri dei job utilizzare `atq`.
> Maggiori informazioni: <https://man.archlinux.org/man/at.1>.

#### Rimuovi il job numero 10:
```shell
atrm {{10}}
```
#### Rimuovi più job, separati da spazi:
```shell
atrm {{15}} {{17}} {{22}}
```
{% endraw %}