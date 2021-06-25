---
layout: default
title: "7za"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="7za">
  <a href="/en/common/7za.html">7za</a> <a href="#7za"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> File archiver with a high compression ratio.
> Similar to `7z` except that it supports fewer file types but is cross-platform.
> More information: <https://www.7-zip.org>.

#### [a]rchive a file or directory:
```shell
7za a {{path/to/archive.7z}} {{path/to/file_or_directory}}
```
#### Encrypt an existing archive (including file names):
```shell
7za a {{path/to/encrypted.7z}} -p{{password}} -mhe=on {{path/to/archive.7z}}
```
#### E[x]tract an archive preserving the original directory structure:
```shell
7za x {{path/to/archive.7z}}
```
#### E[x]tract an archive to a specific directory:
```shell
7za x {{path/to/archive.7z}} -o{{path/to/output}}
```
#### E[x]tract an archive to stdout:
```shell
7za x {{path/to/archive.7z}} -so
```
#### [a]rchive using a specific archive type:
```shell
7z a -t{{7z|zip|gzip|bzip2|lzip}} {{path/to/archive.7z}} {{path/to/file_or_directory}}
```
#### [l]ist the contents of an archive:
```shell
7za l {{path/to/archive.7z}}
```
#### List available archive types:
```shell
7za i
```
{% endraw %}