---
layout: default
title: "unzip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="unzip">
  <a href="/en/common/unzip.html">unzip</a> <a href="#unzip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Extract compressed files in a ZIP archive.

#### Extract zip file(s) (for multiple files, separate file paths by spaces):
```shell
unzip {{file(s)}}
```
#### Extract zip files(s) to given path:
```shell
unzip {{compressed_file(s)}} -d {{path/to/put/extracted_file(s)}}
```
#### List the contents of a zip file without extracting:
```shell
unzip -l {{file.zip}}
```
#### Extract the contents of the file(s) to stdout alongside the extracted file names:
```shell
unzip -c {{file.zip}}
```
#### Extract a zip file created on Windows, containing files with non-ASCII (e.g. Chinese or Japanese characters) filenames:
```shell
unzip -O {{gbk}} {{file.zip}}
```
{% endraw %}