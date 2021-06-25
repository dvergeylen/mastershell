---
layout: default
title: "dpkg-query"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dpkg-query">
  <a href="/en/linux/dpkg-query.html">dpkg-query</a> <a href="#dpkg-query"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool that shows information about installed packages.

#### List all installed packages:
```shell
dpkg-query -l
```
#### List installed packages matching a pattern:
```shell
dpkg-query -l '{{pattern}}'
```
#### List all files installed by a package:
```shell
dpkg-query -L {{package_name}}
```
#### Show information about a package:
```shell
dpkg-query -s {{package_name}}
```
{% endraw %}