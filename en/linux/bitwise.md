---
layout: default
title: "bitwise"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bitwise">
  <a href="/en/linux/bitwise.html">bitwise</a> <a href="#bitwise"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Multi base interactive calculator supporting dynamic base conversion and bit manipulation.
> More information: <https://github.com/mellowcandle/bitwise>.

#### Run using interactive mode:
```shell
bitwise
```
#### Convert from decimal:
```shell
bitwise {{12345}}
```
#### Convert from hexadecimal:
```shell
bitwise {{0x563d}}
```
#### Convert a C-style calculation:
```shell
bitwise "{{0x123 + 0x20 - 30 / 50}}"
```
{% endraw %}