---
layout: default
title: "namei"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="namei">
  <a href="/en/linux/namei.html">namei</a> <a href="#namei"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Follows a pathname (which can be a symbolic link) until a terminal point is found (a file/directory/char device etc).
> This program is useful for finding "too many levels of symbolic links" problems.

#### Resolve the pathnames specified as the argument parameters:
```shell
namei {{path/to/a}} {{path/to/b}} {{path/to/c}}
```
#### Display the results in a long-listing format:
```shell
namei --long {{path/to/a}} {{path/to/b}} {{path/to/c}}
```
#### Show the mode bits of each file type in the style of `ls`:
```shell
namei --modes {{path/to/a}} {{path/to/b}} {{path/to/c}}
```
#### Show owner and group name of each file:
```shell
namei --owners {{path/to/a}} {{path/to/b}} {{path/to/c}}
```
#### Don't follow symlinks while resolving:
```shell
namei --nosymlinks {{path/to/a}} {{path/to/b}} {{path/to/c}}
```
{% endraw %}