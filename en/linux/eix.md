---
layout: default
title: "eix"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="eix">
  <a href="/en/linux/eix.html">eix</a> <a href="#eix"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilities for searching local Gentoo packages.
> Update local package cache using `eix-update`.

#### Search for a package:
```shell
eix {{package_name}}
```
#### Search for installed packages:
```shell
eix --installed {{package_name}}
```
#### Search in package descriptions:
```shell
eix --description "{{description}}"
```
#### Search by package license:
```shell
eix --license {{license}}
```
#### Exclude results from search:
```shell
eix --not --license {{license}}
```
{% endraw %}