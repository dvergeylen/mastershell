---
layout: default
title: "path"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="path">
  <a href="/en/windows/path.html">path</a> <a href="#path"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display or set the search path for executable files.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/path>.

#### Display the current path:
```shell
path
```
#### Set the path to one or more semicolon-separated directories:
```shell
path {{path/to/directory(s)}}
```
#### Append a new directory to the original path:
```shell
path {{path/to/directory}};%path%
```
#### Set command prompt to only search the current directory for executables:
```shell
path ;
```
{% endraw %}