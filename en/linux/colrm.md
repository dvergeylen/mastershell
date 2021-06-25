---
layout: default
title: "colrm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="colrm">
  <a href="/en/linux/colrm.html">colrm</a> <a href="#colrm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove columns from stdin.

#### Remove first column of stdin:
```shell
colrm {{1 1}}
```
#### Remove from 3rd column till the end of each line:
```shell
colrm {{3}}
```
#### Remove from the 3rd column till the 5th column of each line:
```shell
colrm {{3 5}}
```
{% endraw %}