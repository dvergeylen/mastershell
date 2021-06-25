---
layout: default
title: "grex"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="grex">
  <a href="/en/common/grex.html">grex</a> <a href="#grex"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple command-line tool to generate regular expressions.
> More information: <https://github.com/pemistahl/grex>.

#### Generate a simple regular expression:
```shell
 grex {{space_separated_strings}}
```
#### Generate a case-insensitive regular expression:
```shell
grex -i {{space_separated_strings}}
```
#### Replace digits with '\d':
```shell
grex -d {{space_separated_strings}}
```
#### Replace Unicode word character with '\w':
```shell
grex -w {{space_separated_strings}}
```
#### Replace spaces with '\s':
```shell
grex -s {{space_separated_strings}}
```
#### Add {min, max} quantifier representation for repeating sub-strings:
```shell
grex -r {{space_separated_strings}}
```
{% endraw %}