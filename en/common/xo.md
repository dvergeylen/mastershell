---
layout: default
title: "xo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xo">
  <a href="/en/common/xo.html">xo</a> <a href="#xo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A pluggable, zero-configuration linting utility for JavaScript.
> More information: <https://github.com/xojs/xo>.

#### Lint files in the "src" directory:
```shell
xo
```
#### Lint a given set of files:
```shell
xo {{file1}}.js {{file2}}.js
```
#### Automatically fix any lint issues found:
```shell
xo --fix
```
#### Lint using spaces as indentation instead of tabs:
```shell
xo --space
```
#### Lint using the "prettier" code style:
```shell
xo --prettier
```
{% endraw %}