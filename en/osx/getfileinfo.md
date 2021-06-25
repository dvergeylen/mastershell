---
layout: default
title: "GetFileInfo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="getfileinfo">
  <a href="/en/osx/getfileinfo.html">GetFileInfo</a> <a href="#getfileinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get information about a file in an HFS+ directory.

#### Display information about a given file:
```shell
GetFileInfo {{path/to/filename}}
```
#### Display the date and time a given file was created:
```shell
GetFileInfo -d {{path/to/filename}}
```
#### Display the date and time a given file was last modified:
```shell
GetFileInfo -m {{path/to/filename}}
```
#### Display the creator of a given file:
```shell
GetFileInfo -c {{path/to/filename}}
```
{% endraw %}