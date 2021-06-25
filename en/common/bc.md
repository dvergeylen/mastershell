---
layout: default
title: "bc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bc">
  <a href="/en/common/bc.html">bc</a> <a href="#bc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An arbitrary precision calculator language.
> More information: <https://manned.org/bc>.

#### Start `bc` in interactive mode using the standard math library:
```shell
bc -l
```
#### Calculate the result of an expression:
```shell
bc <<< "(1 + 2) * 2 ^ 2"
```
#### Calculate the result of an expression and force the number of decimal places to 10:
```shell
bc <<< "scale=10; 5 / 3"
```
#### Calculate the result of an expression with sine and cosine using `mathlib`:
```shell
bc -l <<< "s(1) + c(1)"
```
{% endraw %}