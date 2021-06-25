---
layout: default
title: "xar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xar">
  <a href="/en/linux/xar.html">xar</a> <a href="#xar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage .xar archives.

#### Create a xar archive of all files in a given directory:
```shell
xar -cf {{archive.xar}} {{path/to/directory}}
```
#### List the contents of a given xar archive:
```shell
xar -tf {{archive.xar}}
```
#### Extract the contents of a given xar archive to the current directory:
```shell
xar -xf {{archive.xar}}
```
{% endraw %}