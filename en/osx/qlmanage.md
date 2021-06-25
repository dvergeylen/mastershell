---
layout: default
title: "qlmanage"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="qlmanage">
  <a href="/en/osx/qlmanage.html">qlmanage</a> <a href="#qlmanage"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> QuickLook server tool.

#### Display QuickLook for one or multiple files:
```shell
qlmanage -p {{filename}} {{filename2}}
```
#### Compute 300px wide PNG thumbnails of all JPEGs in the current directory and put them in a directory:
```shell
qlmanage {{*.jpg}} -t -s {{300}} {{path/to/directory}}
```
#### Reset QuickLook:
```shell
qlmanage -r
```
{% endraw %}