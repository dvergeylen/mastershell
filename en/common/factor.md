---
layout: default
title: "factor"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="factor">
  <a href="/en/common/factor.html">factor</a> <a href="#factor"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Prints the prime factorization of a number.
> More information: <https://www.gnu.org/software/coreutils/factor>.

#### Display the prime-factorization of a number:
```shell
factor {{number}}
```
#### Take the input from stdin if no argument is specified:
```shell
echo {{number}} | factor
```
{% endraw %}