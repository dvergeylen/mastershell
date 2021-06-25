---
layout: default
title: "quilt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="quilt">
  <a href="/en/common/quilt.html">quilt</a> <a href="#quilt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool to manage a series of patches.
> More information: <https://savannah.nongnu.org/projects/quilt>.

#### Import an existing patch from a file:
```shell
quilt import {{path/to/filename.patch}}
```
#### Create a new patch:
```shell
quilt new {{filename.patch}}
```
#### Add a file to the current patch:
```shell
quilt add {{path/to/file}}
```
#### After editing the file, refresh the current patch with the changes:
```shell
quilt refresh
```
#### Apply all the patches in the series file:
```shell
quilt push -a
```
#### Remove all applied patches:
```shell
quilt pop -a
```
{% endraw %}