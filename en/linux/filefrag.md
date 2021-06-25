---
layout: default
title: "filefrag"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="filefrag">
  <a href="/en/linux/filefrag.html">filefrag</a> <a href="#filefrag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Report how badly fragmented a particular file might be.
> More information: <https://manned.org/filefrag>.

#### Display a report for a specific file:
```shell
filefrag {{path/to/file}}
```
#### Display a report for space-separated list of files:
```shell
filefrag {{path/to/file1}} {{path/to/file2}}
```
#### Display a report using a 1024 byte blocksize:
```shell
filefrag -b {{path/to/file}}
```
#### Sync the file before requesting the mapping:
```shell
filefrag -s {{path/to/files}}
```
#### Display mapping of extended attributes:
```shell
filefrag -x {{path/to/files}}
```
#### Display a report with verbose information:
```shell
filefrag -v {{path/to/files}}
```
{% endraw %}