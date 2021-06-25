---
layout: default
title: "git check-ignore"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-check-ignore">
  <a href="/en/common/git-check-ignore.html">git check-ignore</a> <a href="#git-check-ignore"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Analyse and debug Git ignore / exclude (".gitignore") files.
> More information: <https://git-scm.com/docs/git-check-ignore>.

#### Check whether a file or directory is ignored:
```shell
git check-ignore {{path/to/file_or_directory}}
```
#### Check whether multiple files or directories are ignored:
```shell
git check-ignore {{path/to/file}} {{path/to/directory}}
```
#### Use pathnames, one per line, from stdin:
```shell
git check-ignore --stdin < {{path/to/file_list}}
```
#### Do not check the index (used to debug why paths were tracked and not ignored):
```shell
git check-ignore --no-index {{path/to/files_or_directories}}
```
#### Include details about the matching pattern for each path:
```shell
git check-ignore --verbose {{path/to/files_or_directories}}
```
{% endraw %}