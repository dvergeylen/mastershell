---
layout: default
title: "ldconfig"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ldconfig">
  <a href="/en/linux/ldconfig.html">ldconfig</a> <a href="#ldconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Configure symlinks and cache for shared library dependencies.

#### Update symlinks and rebuild the cache (usually run when a new library is installed):
```shell
sudo ldconfig
```
#### Update the symlinks for a given directory:
```shell
sudo ldconfig -n {{path/to/directory}}
```
#### Print the libraries in the cache and check whether a given library is present:
```shell
ldconfig -p | grep {{library_name}}
```
{% endraw %}