---
layout: default
title: "sw_vers"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sw_vers">
  <a href="/en/osx/sw_vers.html">sw_vers</a> <a href="#sw_vers"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print macOS operating system version information.

#### Print all available information (OS name, version number, and build):
```shell
sw_vers
```
#### Print only the version number of the operating system:
```shell
sw_vers -productVersion
```
#### Print only the build identifier:
```shell
sw_vers -buildVersion
```
{% endraw %}