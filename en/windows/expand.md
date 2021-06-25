---
layout: default
title: "expand"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="expand">
  <a href="/en/windows/expand.html">expand</a> <a href="#expand"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Uncompress one or more Windows Cabinet files.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/expand>.

#### Uncompress a single-file Cabinet file to the specified directory:
```shell
expand {{path/to/file.cab}} {{path/to/directory}}
```
#### Display the list of files in a source Cabinet file:
```shell
expand {{path/to/file.cab}} {{path/to/directory}} -d
```
#### Uncompress all files from the Cabinet file:
```shell
expand {{path/to/file.cab}} {{path/to/directory}} -f:*
```
#### Uncompress a specific file from a Cabinet file:
```shell
expand {{path/to/file.cab}} {{path/to/directory}} -f:{{file}}
```
#### Ignore the directory structure when uncompressing, and add them to a single directory:
```shell
expand {{path/to/file.cab}} {{path/to/directory}} -i
```
{% endraw %}