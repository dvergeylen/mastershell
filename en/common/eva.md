---
layout: default
title: "eva"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="eva">
  <a href="/en/common/eva.html">eva</a> <a href="#eva"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple calculator REPL, similar to `bc`, with syntax highlighting and persistent history.
> More information: <https://github.com/NerdyPepper/eva>.

#### Run the calculator in interactive mode:
```shell
eva
```
#### Calculate the result of an expression:
```shell
eva "{{(1 + 2) * 2 ^ 2}}"
```
#### Calculate an expression forcing the number of decimal places to 5:
```shell
eva --fix {{5}} "{{5 / 3}}"
```
#### Calculate an expression with sine and cosine:
```shell
eva "{{sin(1) + cos(1)}}"
```
{% endraw %}