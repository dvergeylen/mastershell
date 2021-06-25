---
layout: default
title: "fdupes"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fdupes">
  <a href="/en/common/fdupes.html">fdupes</a> <a href="#fdupes"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Finds duplicate files in a given set of directories.
> More information: <https://github.com/adrianlopezroche/fdupes>.

#### Search a single directory:
```shell
fdupes {{directory}}
```
#### Search multiple directories:
```shell
fdupes {{directory1}} {{directory2}}
```
#### Search a directory recursively:
```shell
fdupes -r {{directory}}
```
#### Search multiple directories, one recursively:
```shell
fdupes {{directory1}} -R {{directory2}}
```
#### Search recursively for duplicates and display interactive prompt to pick which ones to keep, deleting the others:
```shell
fdupes -rd {{directory}}
```
#### Search recursively and delete duplicates without prompting:
```shell
fdupes -rdN {{directory}}
```
{% endraw %}