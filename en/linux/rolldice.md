---
layout: default
title: "rolldice"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rolldice">
  <a href="/en/linux/rolldice.html">rolldice</a> <a href="#rolldice"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Roll virtual dice.
> More information: <https://manned.org/rolldice>.

#### Roll a single 20 sided dice:
```shell
rolldice d{{20}}
```
#### Roll two six sided dice and drop the lowest roll:
```shell
rolldice {{2}}d{{6}}s{{1}}
```
#### Roll two 20 sided dice and add a modifier value:
```shell
rolldice {{2}}d{{20}}{{+5}}
```
#### Roll a 20 sided dice two times:
```shell
rolldice {{2}}xd{{20}}
```
{% endraw %}