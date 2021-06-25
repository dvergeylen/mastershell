---
layout: default
title: "qmv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="qmv">
  <a href="/en/common/qmv.html">qmv</a> <a href="#qmv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Move files and directories using the default text editor to define the filenames.
> More information: <https://www.nongnu.org/renameutils/>.

#### Move a single file (open an editor with the source filename on the left and the target filename on the right):
```shell
qmv {{source_file}}
```
#### Move multiple JPG files:
```shell
qmv {{*.jpg}}
```
#### Move multiple directories:
```shell
qmv -d {{path/to/directory1}} {{path/to/directory2}} {{path/to/directory3}}
```
#### Move all files and directories inside a directory:
```shell
qmv --recursive {{path/to/directory}}
```
#### Move files, but swap the positions of the source and the target filenames in the editor:
```shell
qmv --option swap {{*.jpg}}
```
{% endraw %}