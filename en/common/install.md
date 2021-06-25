---
layout: default
title: "install"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="install">
  <a href="/en/common/install.html">install</a> <a href="#install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copy files and set attributes.
> Copy files (often executable) to a system location like `/usr/local/bin`, give them the appropriate permissions/ownership.
> More information: <https://www.gnu.org/software/coreutils/install>.

#### Copy files to destination:
```shell
install {{path/to/source}} {{path/to/destination}}
```
#### Copy files to destination, setting their ownership:
```shell
install -o {{user}} {{path/to/source}} {{path/to/destination}}
```
#### Copy files to destination, setting their group ownership:
```shell
install -g {{user}} {{path/to/source}} {{path/to/destination}}
```
#### Copy files to destination, setting their `mode`:
```shell
install -m {{+x}} {{path/to/source}} {{path/to/destination}}
```
#### Copy files and apply access/modification times of source to destination:
```shell
install -p {{path/to/source}} {{path/to/destination}}
```
{% endraw %}