---
layout: default
title: "srm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="srm">
  <a href="/en/common/srm.html">srm</a> <a href="#srm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Securely remove files or directories.
> Overwrites the existing data one or multiple times. Drop in replacement for rm.
> More information: <http://srm.sourceforge.net/srm.html>.

#### Remove a file after a single-pass overwriting with random data:
```shell
srm -s {{path/to/file}}
```
#### Remove a file after seven passes of overwriting with random data:
```shell
srm -m {{path/to/file}}
```
#### Recursively remove a directory and its contents overwriting each file with a single-pass of random data:
```shell
srm -r -s {{path/to/directory}}
```
#### Prompt before every removal:
```shell
srm -i {{\*}}
```
{% endraw %}