---
layout: default
title: "eslint"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="eslint">
  <a href="/pl/common/eslint.html">eslint</a> <a href="#eslint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Podłączane narzędzie lintowania dla JavaScript i JSX.
> Więcej informacji: <https://eslint.org>.

#### Stwórz eslint config:
```shell
eslint --init
```
#### Lint na danym zestawie plików:
```shell
eslint {{nazwapliku}}.js {{nazwapliku1}}.js
```
#### Napraw lint issues:
```shell
eslint --fix
```
#### Lint z config:
```shell
eslint -c {{sciezka/do/pliku_config}} {{app/src}}
```
{% endraw %}