---
layout: default
title: "base64"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="base64">
  <a href="/en/osx/base64.html">base64</a> <a href="#base64"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Encode and decode using Base64 representation.

#### Encode a file:
```shell
base64 --input={{plain_file}}
```
#### Decode a file:
```shell
base64 --decode --input={{base64_file}}
```
#### Encode from stdin:
```shell
echo -n {{plain_text}} | base64
```
#### Decode from stdin:
```shell
echo -n {{base64_text}} | base64 --decode
```
{% endraw %}