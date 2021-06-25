---
layout: default
title: "yaa"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="yaa">
  <a href="/en/osx/yaa.html">yaa</a> <a href="#yaa"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create and manipulate YAA archives.

#### Create an archive from a directory:
```shell
yaa archive -d {{path/to/directory}} -o {{path/to/output.yaa}}
```
#### Create an archive from a file:
```shell
yaa archive -i {{path/to/file}} -o {{path/to/output.yaa}}
```
#### Extract an archive to the current directory:
```shell
yaa extract -i {{path/to/archive.yaa}}
```
#### List the contents of an archive:
```shell
yaa list -i {{path/to/archive.yaa}}
```
#### Create an archive with a specific compression algorithm:
```shell
yaa archive -a {{algorithm}} -d {{path/to/directory}} -o {{path/to/output.yaa}}
```
#### Create an archive with an 8MB block size:
```shell
yaa archive -b {{8m}} -d {{path/to/directory}} -o {{path/to/output.yaa}}
```
{% endraw %}