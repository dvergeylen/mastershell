---
layout: default
title: "scoop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="scoop">
  <a href="/en/windows/scoop.html">scoop</a> <a href="#scoop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line installer for Windows.
> More information: <https://scoop.sh>.

#### Install a package:
```shell
scoop install {{package}}
```
#### Remove a package:
```shell
scoop uninstall {{package}}
```
#### Update all installed packages:
```shell
scoop update *
```
#### List installed packages:
```shell
scoop list
```
#### Display information about a package:
```shell
scoop info {{package}}
```
#### Search for a package:
```shell
scoop search {{package}}
```
#### Remove old versions of all packages and clear the download cache:
```shell
scoop cleanup -k *
```
{% endraw %}