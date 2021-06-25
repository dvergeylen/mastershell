---
layout: default
title: "kjv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kjv">
  <a href="/en/linux/kjv.html">kjv</a> <a href="#kjv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The word of God available right on your desktop.
> More information: <https://github.com/bontibon/kjv>.

#### Display books:
```shell
kjv -l
```
#### Open a specific book:
```shell
kjv {{Genesis}}
```
#### Open a specific chapter of a book:
```shell
kjv {{Genesis}} {{2}}
```
#### Open a specific verse of a specific chapter of a book:
```shell
kjv {{John}} {{3}}:{{16}}
```
#### Open a specific range of verses of a book's chapter:
```shell
kjv {{Proverbs}} {{3}}:{{1-6}}
```
#### Display a specific range of verses of a book from different chapters:
```shell
kjv {{Matthew}} {{1}}:{{7}}-{{2}}:{{6}}
```
#### Display all verses that match a pattern:
```shell
kjv /{{Plagues}}
```
#### Display all verses that match a pattern in a specific book:
```shell
kjv {{1Jn}}/{{antichrist}}
```
{% endraw %}