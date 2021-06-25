---
layout: default
title: "dpkg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dpkg">
  <a href="/en/linux/dpkg.html">dpkg</a> <a href="#dpkg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian package manager.
> More information: <https://manpages.debian.org/buster/dpkg/dpkg.1.en.html>.

#### Install a package:
```shell
dpkg -i {{path/to/file.deb}}
```
#### Remove a package:
```shell
dpkg -r {{package_name}}
```
#### List installed packages:
```shell
dpkg -l {{pattern}}
```
#### List a package's contents:
```shell
dpkg -L {{package_name}}
```
#### List contents of a local package file:
```shell
dpkg -c {{path/to/file.deb}}
```
#### Find out which package owns a file:
```shell
dpkg -S {{filename}}
```
{% endraw %}