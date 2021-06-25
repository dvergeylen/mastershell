---
layout: default
title: "robocopy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="robocopy">
  <a href="/en/windows/robocopy.html">robocopy</a> <a href="#robocopy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Robust File and Folder Copy.
> By default files will only be copied if the source and destination have different time stamps or different file sizes.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/robocopy>.

#### Copy all `.jpg` and `.bmp` files from one directory to another:
```shell
robocopy {{path/to/source}} {{path/to/destination}} {{*.jpg}} {{*.bmp}}
```
#### Copy all files and subdirectories, including empty ones:
```shell
robocopy {{path/to/source}} {{path/to/destination}} /E
```
#### Mirror/Sync a directory, deleting anything not in source and include all attributes and permissions:
```shell
robocopy {{path/to/source}} {{path/to/destination}} /MIR /COPYALL
```
#### Copy all files and subdirectories, excluding source files that are older than destination files:
```shell
robocopy {{path/to/source}} {{path/to/destination}} /E /XO
```
#### List all files 50 MBytes or larger in size instead of copying them:
```shell
robocopy {{path/to/source}} {{path/to/destination}} /MIN:52428800 /L
```
#### Allow resuming if network connection is lost and limit retries to 5 and wait time to 15 sec:
```shell
robocopy {{path/to/source}} {{path/to/destination}} /Z /R:5 /W:15
```
#### Display detailed usage information:
```shell
robocopy /?
```
{% endraw %}