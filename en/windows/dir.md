---
layout: default
title: "dir"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dir">
  <a href="/en/windows/dir.html">dir</a> <a href="#dir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List directory contents.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/dir>.

#### Show the contents of the current directory:
```shell
dir
```
#### Show the contents of a given directory:
```shell
dir {{path/to/directory}}
```
#### Show the contents of the current directory, including hidden ones:
```shell
dir /A
```
#### Show the contents of a given directory, including hidden ones:
```shell
dir {{path/to/directory}} /A
```
{% endraw %}