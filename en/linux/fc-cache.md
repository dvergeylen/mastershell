---
layout: default
title: "fc-cache"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fc-cache">
  <a href="/en/linux/fc-cache.html">fc-cache</a> <a href="#fc-cache"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Scan font directories in order to build font cache files.

#### Generate font cache files:
```shell
fc-cache
```
#### Force a rebuild of all font cache files, without checking if cache is up-to-date:
```shell
fc-cache -f
```
#### Erase font cache files, then generate new font cache files:
```shell
fc-cache -r
```
{% endraw %}