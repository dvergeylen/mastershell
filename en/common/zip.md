---
layout: default
title: "zip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zip">
  <a href="/en/common/zip.html">zip</a> <a href="#zip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Package and compress (archive) files into zip file.

#### Package and compress files and directories [r]ecursively:
```shell
zip -r {{compressed.zip}} {{path/to/file}} {{path/to/directory1}} {{path/to/directory2}}
```
#### E[x]clude unwanted files from being added to the compressed archive:
```shell
zip -r {{compressed.zip}} {{path/to/directory}} -x {{path/to/exclude}}
```
#### Archive a directory and its contents with the highest level [9] of compression:
```shell
zip -r -{{9}} {{compressed.zip}} {{path/to/directory}}
```
#### Create an encrypted archive (user will be prompted for a password):
```shell
zip -e -r {{compressed.zip}} {{path/to/directory}}
```
#### Add files to an existing zip file:
```shell
zip {{compressed.zip}} {{path/to/file}}
```
#### Delete files from an existing zip file:
```shell
zip -d {{compressed.zip}} "{{foo/*.tmp}}"
```
#### Archive a directory and its contents to a multi-part [s]plit zip file (e.g. 3GB parts):
```shell
zip -r -s {{3g}} {{compressed.zip}} {{path/to/directory}}
```
#### List files within a specified archive (without extracting them):
```shell
zip -sf {{compressed.zip}}
```
{% endraw %}