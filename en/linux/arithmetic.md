---
layout: default
title: "arithmetic"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="arithmetic">
  <a href="/en/linux/arithmetic.html">arithmetic</a> <a href="#arithmetic"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Quiz on simple arithmetic problems.
> More information: <https://manpages.debian.org/bsdgames/arithmetic.6.en.html>.

#### Start an arithmetic quiz:
```shell
arithmetic
```
#### Specify one or more arithmetic [o]peration symbols to get problems on them:
```shell
arithmetic -o {{+|-|x|/}}
```
#### Specify a range. Addition and multiplication problems would feature numbers between 0 and range, inclusive. Subtraction and division problems would have required result and number to be operated on, between 0 and range:
```shell
arithmetic -r {{7}}
```
{% endraw %}