---
layout: default
title: "cradle package"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cradle-package">
  <a href="/en/common/cradle-package.html">cradle package</a> <a href="#cradle-package"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage packages for a Cradle instance.
> More information: <https://cradlephp.github.io/docs/3.B.-Reference-Command-Line-Tools.html#package>.

#### Display a list of available packages:
```shell
cradle package list
```
#### Search for a package:
```shell
cradle package search {{package}}
```
#### Install a package from Packagist:
```shell
cradle package install {{package}}
```
#### Install a specific version of a package:
```shell
cradle package install {{package}} {{version}}
```
#### Update a package:
```shell
cradle package update {{package}}
```
#### Update a package to a specific version:
```shell
cradle package update {{package}} {{version}}
```
#### Remove a specific package:
```shell
cradle package remove {{package}}
```
{% endraw %}