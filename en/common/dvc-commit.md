---
layout: default
title: "dvc commit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dvc-commit">
  <a href="/en/common/dvc-commit.html">dvc commit</a> <a href="#dvc-commit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Record changes to DVC-tracked files in the project.
> More information: <https://dvc.org/doc/command-reference/commit>.

#### Commit changes to all DVC-tracked files and directories:
```shell
dvc commit
```
#### Commit changes to a specified DVC-tracked target:
```shell
dvc commit {{target}}
```
#### Recursively commit all DVC-tracked files in a directory:
```shell
dvc commit --recursive {{path/to/directory}}
```
{% endraw %}