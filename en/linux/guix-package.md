---
layout: default
title: "guix package"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="guix-package">
  <a href="/en/linux/guix-package.html">guix package</a> <a href="#guix-package"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Install, upgrade and remove Guix packages, or rollback to previous configurations.

#### Install a new package:
```shell
guix package -i {{package_name}}
```
#### Remove a package:
```shell
guix package -r {{package_name}}
```
#### Search the package database for a regular expression:
```shell
guix package -s "{{search_pattern}}"
```
#### List installed packages:
```shell
guix package -I
```
#### List generations:
```shell
guix package -l
```
#### Roll back to the previous generation:
```shell
guix package --roll-back
```
{% endraw %}