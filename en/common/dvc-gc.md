---
layout: default
title: "dvc gc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dvc-gc">
  <a href="/en/common/dvc-gc.html">dvc gc</a> <a href="#dvc-gc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove unused files and directories from the cache or remote storage.
> More information: <https://dvc.org/doc/command-reference/gc>.

#### Garbage collect from the cache, keeping only versions referenced by the current workspace:
```shell
dvc gc --workspace
```
#### Garbage collect from the cache, keeping only versions referenced by branch, tags, and commits:
```shell
dvc gc --all-branches --all-tags --all-commits
```
#### Garbage collect from the cache, including the default cloud remote storage (if set):
```shell
dvc gc --all-commits --cloud
```
#### Garbage collect from the cache, including a specific cloud remote storage:
```shell
dvc gc --all-commits --cloud --remote {{remote_name}}
```
{% endraw %}