---
layout: default
title: "mv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mv">
  <a href="/en/common/mv.html">mv</a> <a href="#mv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Move or rename files and directories.
> More information: <https://www.gnu.org/software/coreutils/mv>.

#### Move a file to an arbitrary location:
```shell
mv {{source}} {{target}}
```
#### Move files into another directory, keeping the filenames:
```shell
mv {{source1}} {{source2}} {{source3}} {{target_directory}}
```
#### Do not prompt for confirmation before overwriting existing files:
```shell
mv -f {{source}} {{target}}
```
#### Prompt for confirmation before overwriting existing files, regardless of file permissions:
```shell
mv -i {{source}} {{target}}
```
#### Do not overwrite existing files at the target:
```shell
mv -n {{source}} {{target}}
```
#### Move files in verbose mode, showing files after they are moved:
```shell
mv -v {{source}} {{target}}
```
{% endraw %}