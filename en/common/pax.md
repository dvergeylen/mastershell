---
layout: default
title: "pax"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pax">
  <a href="/en/common/pax.html">pax</a> <a href="#pax"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Archiving and copying utility.

#### List the contents of an archive:
```shell
pax -f {{archive.tar}}
```
#### List the contents of a gzipped archive:
```shell
pax -zf {{archive.tar.gz}}
```
#### Create an archive from files:
```shell
pax -wf {{target.tar}} {{path/to/file1}} {{path/to/file2}} {{path/to/file3}}
```
#### Create an archive from files, using output redirection:
```shell
pax -w {{path/to/file1}} {{path/to/file2}} {{path/to/file3}} > {{target.tar}}
```
#### Extract an archive into the current directory:
```shell
pax -rf {{source.tar}}
```
#### Copy to a directory, while keeping the original metadata; `target/` must exist:
```shell
pax -rw {{path/to/file1}} {{path/to/directory1}} {{path/to/directory2}} {{target/}}
```
{% endraw %}