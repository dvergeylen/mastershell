---
layout: default
title: "pkgadd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pkgadd">
  <a href="/en/linux/pkgadd.html">pkgadd</a> <a href="#pkgadd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Add a package to a CRUX system.

#### Install a local software package:
```shell
pkgadd {{package_name}}
```
#### Update an already installed package from a local package:
```shell
pkgadd -u {{package_name}}
```
{% endraw %}