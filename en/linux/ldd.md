---
layout: default
title: "ldd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ldd">
  <a href="/en/linux/ldd.html">ldd</a> <a href="#ldd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display shared library dependencies.

#### Display shared library dependencies of a binary:
```shell
ldd {{path/to/binary}}
```
#### Display unused direct dependencies:
```shell
ldd -u {{path/to/binary}}
```
{% endraw %}