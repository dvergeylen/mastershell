---
layout: default
title: "dpkg-deb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dpkg-deb">
  <a href="/en/linux/dpkg-deb.html">dpkg-deb</a> <a href="#dpkg-deb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pack, unpack and provide information about Debian archives.
> More information: <https://manpages.debian.org/buster/dpkg/dpkg-deb.1.en.html>.

#### Display information about a package:
```shell
dpkg-deb --info {{path/to/file.deb}}
```
#### Display the package's name and version on one line:
```shell
dpkg-deb --show {{path/to/file.deb}}
```
#### List the package's contents:
```shell
dpkg-deb --contents {{path/to/file.deb}}
```
#### Extract package's contents into a directory:
```shell
dpkg-deb --extract {{path/to/file.deb}} {{path/to/directory}}
```
#### Create a package from a specified directory:
```shell
dpkg-deb --build {{path/to/directory}}
```
{% endraw %}