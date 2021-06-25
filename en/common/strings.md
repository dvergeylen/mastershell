---
layout: default
title: "strings"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="strings">
  <a href="/en/common/strings.html">strings</a> <a href="#strings"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Find printable strings in an object file or binary.

#### Print all strings in a binary:
```shell
strings {{file}}
```
#### Limit results to strings at least *length* characters long:
```shell
strings -n {{length}} {{file}}
```
#### Prefix each result with its offset within the file:
```shell
strings -t d {{file}}
```
#### Prefix each result with its offset within the file in hexadecimal:
```shell
strings -t x {{file}}
```
{% endraw %}