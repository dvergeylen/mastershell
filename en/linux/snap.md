---
layout: default
title: "snap"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="snap">
  <a href="/en/linux/snap.html">snap</a> <a href="#snap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for managing the "snap" self-contained software packages.
> Similar to what `apt` is for ".deb".

#### Search for a package:
```shell
snap find {{package_name}}
```
#### Install a package:
```shell
snap install {{package_name}}
```
#### Update a package:
```shell
snap refresh {{package_name}}
```
#### Update a package to another channel (track, risk, or branch):
```shell
snap refresh {{package_name}} --channel={{channel}}
```
#### Update all packages:
```shell
snap refresh
```
#### Display basic information about installed snap software:
```shell
snap list
```
#### Uninstall a package:
```shell
snap remove {{package_name}}
```
#### Check for recent snap changes in the system:
```shell
snap changes
```
{% endraw %}