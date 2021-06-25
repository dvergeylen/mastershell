---
layout: default
title: "fileicon"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fileicon">
  <a href="/en/osx/fileicon.html">fileicon</a> <a href="#fileicon"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A macOS CLI to manage custom file and folder icons.
> More information: <https://github.com/mklement0/fileicon>.

#### Set a custom icon for a specific file or directory:
```shell
fileicon set {{path/to/file_or_directory}} {{path/to/icon.png}}
```
#### Remove a custom icon from a specific file or directory:
```shell
fileicon rm {{path/to/file_or_directory}}
```
#### Save the custom icon of a file or directory as a `.icns` file into the current directory:
```shell
fileicon get {{path/to/file_or_directory}}
```
#### Test if a specific file or directory has a custom icon:
```shell
fileicon test {{path/to/file_or_directory}}
```
{% endraw %}