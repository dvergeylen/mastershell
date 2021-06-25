---
layout: default
title: "unar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="unar">
  <a href="/en/common/unar.html">unar</a> <a href="#unar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Extract contents from archive files.

#### Extract an archive to the current directory:
```shell
unar {{archive}}
```
#### Extract an archive to the specified directory:
```shell
unar -o {{path/to/directory}} {{archive}}
```
#### Force overwrite if files to be unpacked already exist:
```shell
unar -f {{archive}}
```
#### Force rename if files to be unpacked already exist:
```shell
unar -r {{archive}}
```
#### Force skip if files to be unpacked already exist:
```shell
unar -s {{archive}}
```
{% endraw %}