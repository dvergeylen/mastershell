---
layout: default
title: "p7zip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="p7zip">
  <a href="/en/common/p7zip.html">p7zip</a> <a href="#p7zip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wrapper of 7-Zip file archiver with high compression ratio.
> Internally executes either 7za or 7zr command.
> More information: <http://p7zip.sourceforge.net>.

#### Archive a file, replacing it with a 7zipped compressed version:
```shell
p7zip {{path/to/file}}
```
#### Archive a file keeping the input file:
```shell
p7zip -k {{path/to/file}}
```
#### Decompress a file, replacing it with the original uncompressed version:
```shell
p7zip -d {{compressed.ext}}.7z
```
#### Decompress a file keeping the input file:
```shell
p7zip -d -k {{compressed.ext}}.7z
```
#### Skip some checks and force compression or decompression:
```shell
p7zip -f {{path/to/file}}
```
{% endraw %}