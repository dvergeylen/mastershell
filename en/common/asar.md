---
layout: default
title: "asar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="asar">
  <a href="/en/common/asar.html">asar</a> <a href="#asar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A file archiver for the Electron platform.
> More information: <https://github.com/electron/asar>.

#### Archive a file or directory:
```shell
asar pack {{path/to/file_or_directory}} {{archived.asar}}
```
#### Extract an archive:
```shell
asar extract {{archived.asar}}
```
#### Extract a specific file from an archive:
```shell
asar extract-file {{archived.asar}} {{file}}
```
#### List the contents of an archive file:
```shell
asar list {{archived.asar}}
```
{% endraw %}