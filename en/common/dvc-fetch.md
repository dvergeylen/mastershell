---
layout: default
title: "dvc fetch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dvc-fetch">
  <a href="/en/common/dvc-fetch.html">dvc fetch</a> <a href="#dvc-fetch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Download DVC tracked files and directories from a remote repository.
> More information: <https://dvc.org/doc/command-reference/fetch>.

#### Fetch the latest changes from the default remote upstream repository (if set):
```shell
dvc fetch
```
#### Fetch changes from a specific remote upstream repository:
```shell
dvc fetch --remote {{remote_name}}
```
#### Fetch the latest changes for a specific target/s:
```shell
dvc fetch {{target/s}}
```
#### Fetch changes for all branch and tags:
```shell
dvc fetch --all-branches --all-tags
```
#### Fetch changes for all commits:
```shell
dvc fetch --all-commits
```
{% endraw %}