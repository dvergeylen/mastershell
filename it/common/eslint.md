---
layout: default
title: "eslint"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="eslint">
  <a href="/it/common/eslint.html">eslint</a> <a href="#eslint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilità di linting per JavaScript e JSX.
> Maggiori informazioni: <https://eslint.org>.

#### Crea una configurazione eslint:
```shell
eslint --init
```
#### Esegui il linting di un dato set di file:
```shell
eslint {{file1.js file2.js}}
```
#### Risolvi gli errori di linting:
```shell
eslint --fix
```
#### Esegui il linting utilizzando un determinato file di configurazione:
```shell
eslint -c {{percorso/a/file_config}} {{app/src}}
```
{% endraw %}