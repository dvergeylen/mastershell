---
layout: default
title: "eslint"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="eslint">
  <a href="/en/common/eslint.html">eslint</a> <a href="#eslint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A pluggable linting utility for JavaScript and JSX.
> More information: <https://eslint.org>.

#### Create eslint config:
```shell
eslint --init
```
#### Lint on a given set of files:
```shell
eslint {{filename}}.js {{filename1}}.js
```
#### Fix lint issues:
```shell
eslint --fix
```
#### Lint with config:
```shell
eslint -c {{path/to/config_file}} {{app/src}}
```
{% endraw %}