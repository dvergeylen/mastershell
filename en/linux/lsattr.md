---
layout: default
title: "lsattr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lsattr">
  <a href="/en/linux/lsattr.html">lsattr</a> <a href="#lsattr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List file attributes on a Linux filesystem.

#### Display the attributes of the files in the current directory:
```shell
lsattr
```
#### List the attributes of files in a particular path:
```shell
lsattr {{path}}
```
#### List file attributes recursively in the current and subsequent directories:
```shell
lsattr -R
```
#### Show attributes of all the files in the current directory, including hidden ones:
```shell
lsattr -a
```
#### Display attributes of directories in the current directory:
```shell
lsattr -d
```
{% endraw %}