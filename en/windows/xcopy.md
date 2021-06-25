---
layout: default
title: "xcopy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xcopy">
  <a href="/en/windows/xcopy.html">xcopy</a> <a href="#xcopy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copy files and directory trees.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/xcopy>.

#### Copy the file(s) to the specified destination:
```shell
xcopy {{path/to/file_or_directory}} {{path/to/destination}}
```
#### List files that will be copied before copying:
```shell
xcopy {{path/to/file_or_directory}} {{path/to/destination}} /p
```
#### Copy the directory structure only, excluding files:
```shell
xcopy {{path/to/file_or_directory}} {{path/to/destination}} /t
```
#### Include empty directories when copying:
```shell
xcopy {{path/to/file_or_directory}} {{path/to/destination}} /e
```
#### Keep the source ACL in the destination:
```shell
xcopy {{path/to/file_or_directory}} {{path/to/destination}} /o
```
#### Allow resuming when network connection is lost:
```shell
xcopy {{path/to/file_or_directory}} {{path/to/destination}} /z
```
#### Disable the prompt when the file exists in the destination:
```shell
xcopy {{path/to/file_or_directory}} {{path/to/destination}} /y
```
#### Display detailed usage information:
```shell
xcopy /?
```
{% endraw %}