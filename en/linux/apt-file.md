---
layout: default
title: "apt-file"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-file">
  <a href="/en/linux/apt-file.html">apt-file</a> <a href="#apt-file"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Search for files in apt packages, including ones not yet installed.
> More information: <https://manpages.debian.org/latest/apt-file/apt-file.1.html>.

#### Update the metadata database:
```shell
sudo apt update
```
#### Search for packages that contain the specified file or path:
```shell
apt-file {{search|find}} {{part/of/filename}}
```
#### List the contents of a specific package:
```shell
apt-file {{show|list}} {{package_name}}
```
#### Search for packages that match the regular expression given in `pattern`:
```shell
apt-file {{search|find}} --regexp {{regular_expression}}
```
{% endraw %}