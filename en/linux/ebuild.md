---
layout: default
title: "ebuild"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ebuild">
  <a href="/en/linux/ebuild.html">ebuild</a> <a href="#ebuild"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A low level interface to the Gentoo Portage system.

#### Create or update the package manifest:
```shell
ebuild {{path/to/file.ebuild}} manifest
```
#### Clean the temporary build directories for the build file:
```shell
ebuild {{path/to/file.ebuild}} clean
```
#### Fetch sources if they do not exist:
```shell
ebuild {{path/to/file.ebuild}} fetch
```
#### Extract the sources to a temporary build directory:
```shell
ebuild {{path/to/file.ebuild}} unpack
```
#### Compile the extracted sources:
```shell
ebuild {{path/to/file.ebuild}} compile
```
#### Install the package to a temporary install directory:
```shell
ebuild {{path/to/file.ebuild}} install
```
#### Install the temporary files to the live filesystem:
```shell
ebuild {{path/to/file.ebuild}} qmerge
```
#### Fetch, unpack, compile, install and qmerge the specified ebuild file:
```shell
ebuild {{path/to/file.ebuild}} merge
```
{% endraw %}