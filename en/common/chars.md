---
layout: default
title: "chars"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chars">
  <a href="/en/common/chars.html">chars</a> <a href="#chars"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display names and codes for various ASCII and Unicode characters and code points.
> More information: <https://github.com/antifuchs/chars>.

#### Look up a character by its value:
```shell
chars '{{ß}}'
```
#### Look up a character by its Unicode code point:
```shell
chars {{U+1F63C}}
```
#### Look up possible characters given an ambiguous code point:
```shell
chars {{10}}
```
#### Look up a control character:
```shell
chars "{{^C}}"
```
{% endraw %}