---
layout: default
title: "jdupes"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jdupes">
  <a href="/en/common/jdupes.html">jdupes</a> <a href="#jdupes"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A powerful duplicate file finder and an enhanced fork of fdupes.
> More information: <https://github.com/jbruchon/jdupes>.

#### Search a single directory:
```shell
jdupes {{directory}}
```
#### Search multiple directories:
```shell
jdupes {{directory1}} {{directory2}}
```
#### Search all directories recursively:
```shell
jdupes --recurse {{directory}}
```
#### Search directory recursively and let user choose files to preserve:
```shell
jdupes --delete --recurse {{directory}}
```
#### Search multiple directories and follow subdirectores under directory2, not directory1:
```shell
jdupes {{directory1}} --recurse: {{directory2}}
```
#### Search multiple directories and keep the directory order in result:
```shell
jdupes -O {{directory1}} {{directory2}} {{directory3}}
```
{% endraw %}