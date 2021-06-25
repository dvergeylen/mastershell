---
layout: default
title: "equery"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="equery">
  <a href="/en/linux/equery.html">equery</a> <a href="#equery"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> View information about Portage packages.

#### List all installed packages:
```shell
equery list '*'
```
#### Search for installed packages in the Portage tree and in overlays:
```shell
equery list -po {{package_name}}
```
#### List all packages that depend on a given package:
```shell
equery depends {{package_name}}
```
#### List all packages that a given package depends on:
```shell
equery depgraph {{package_name}}
```
#### List all files installed by a package:
```shell
equery files --tree {{package_name}}
```
{% endraw %}