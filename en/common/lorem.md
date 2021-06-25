---
layout: default
title: "lorem"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lorem">
  <a href="/en/common/lorem.html">lorem</a> <a href="#lorem"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create more or less random lorem ipsum text.

#### Print the specified number of words:
```shell
lorem -n {{20}}
```
#### Print 10 lines of Goethe's Faust:
```shell
lorem -l {{10}} --faust
```
#### Print 5 sentences of Poe's Raven:
```shell
lorem -s {{5}} --raven
```
#### Print 40 random characters from Boccacio's Decameron:
```shell
lorem --randomize -c {{40}} --decamerone
```
{% endraw %}