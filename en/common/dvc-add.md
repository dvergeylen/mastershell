---
layout: default
title: "dvc add"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dvc-add">
  <a href="/en/common/dvc-add.html">dvc add</a> <a href="#dvc-add"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Add changed files to the index.
> More information: <https://dvc.org/doc/command-reference/add>.

#### Add a single target file to the index:
```shell
dvc add {{path/to/file}}
```
#### Add a target directory to the index:
```shell
dvc add {{path/to/directory}}
```
#### Recursively add all the files in a given target directory:
```shell
dvc add --recursive {{path/to/directory}}
```
#### Add a target file with a custom `.dvc` filename:
```shell
dvc add --file {{custom_name.dvc}} {{path/to/file}}
```
{% endraw %}