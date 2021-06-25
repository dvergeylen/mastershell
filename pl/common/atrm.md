---
layout: default
title: "atrm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="atrm">
  <a href="/pl/common/atrm.html">atrm</a> <a href="#atrm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Usuwa zadania o zadanych identyfikatorach (numerach) wcześniej zakolejkowane przez `at` lub `batch`
> Aby znaleźć numery zadań, użyj `atq`.
> Więcej informacji: <https://man.archlinux.org/man/at.1>.

#### Usuń zadanie numer 10:
```shell
atrm {{10}}
```
#### Usuń kilka zadań, oddzielonych spacjami:
```shell
atrm {{15}} {{17}} {{22}}
```
{% endraw %}