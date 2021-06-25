---
layout: default
title: "replace"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="replace">
  <a href="/en/windows/replace.html">replace</a> <a href="#replace"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Replace files.
> See also: `robocopy`, `move`, `copy`, and `del`.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/replace>.

#### Replace the destination file with the one from the source directory:
```shell
replace {{path/to/file_or_directory}} {{path/to/destination}}
```
#### Add files to the destination directory instead of replacing existing files:
```shell
replace {{path/to/file_or_directory}} {{path/to/destination}} /a
```
#### Interactively copy multiple files, with a prompt before replacing or adding a destination file:
```shell
replace {{path/to/file_or_directory}} {{path/to/destination}} /p
```
#### Replace even read only files:
```shell
replace {{path/to/file_or_directory}} {{path/to/destination}} /r
```
#### Wait for you to insert a disk before it replaces files (originally to allow inserting a floppy disk):
```shell
replace {{path/to/file_or_directory}} {{path/to/destination}} /w
```
#### Replace all files in subdirectories of the destination:
```shell
replace {{path/to/file_or_directory}} {{path/to/destination}} /s
```
#### Replace only files in the destination directory which are older than the files in the source directory:
```shell
replace {{path/to/file_or_directory}} {{path/to/destination}} /u
```
#### Display detailed usage information:
```shell
replace /?
```
{% endraw %}