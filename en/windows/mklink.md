---
layout: default
title: "mklink"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mklink">
  <a href="/en/windows/mklink.html">mklink</a> <a href="#mklink"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create symbolic links.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/mklink>.

#### Create a symbolic link to a file:
```shell
mklink {{path/to/link}} {{path/to/source_file}}
```
#### Create a symbolic link to a directory:
```shell
mklink /d {{path/to/link}} {{path/to/source_directory}}
```
#### Create a hard link to a file:
```shell
mklink /h {{path/to/link}} {{path/to/source_file}}
```
#### Create a directory junction:
```shell
mklink /j {{path/to/link}} {{path/to/source_file}}
```
{% endraw %}