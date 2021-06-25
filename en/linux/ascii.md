---
layout: default
title: "ascii"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ascii">
  <a href="/en/linux/ascii.html">ascii</a> <a href="#ascii"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show ASCII character aliases.
> More information: <http://www.catb.org/~esr/ascii/>.

#### Show ASCII aliases of a character:
```shell
ascii {{a}}
```
#### Show ASCII aliases in short, script-friendly mode:
```shell
ascii -t {{a}}
```
#### Show ASCII aliases of multiple characters:
```shell
ascii -s {{tldr}}
```
#### Show ASCII table in decimal:
```shell
ascii -d
```
#### Show ASCII table in hexadecimal:
```shell
ascii -x
```
#### Show ASCII table in octal:
```shell
ascii -o
```
#### Show ASCII table in binary:
```shell
ascii -b
```
#### Show options summary and complete ASCII table:
```shell
ascii
```
{% endraw %}