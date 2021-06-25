---
layout: default
title: "unexpand"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="unexpand">
  <a href="/en/common/unexpand.html">unexpand</a> <a href="#unexpand"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert spaces to tabs.
> More information: <https://www.gnu.org/software/coreutils/unexpand>.

#### Convert blanks in each file to tabs, writing to standard output:
```shell
unexpand {{file}}
```
#### Convert blanks to tabs, reading from standard output:
```shell
unexpand
```
#### Convert all blanks, instead of just initial blanks:
```shell
unexpand -a {{file}}
```
#### Convert only leading sequences of blanks (overrides -a):
```shell
unexpand --first-only {{file}}
```
#### Have tabs a certain number of characters apart, not 8 (enables -a):
```shell
unexpand -t {{number}} {{file}}
```
{% endraw %}