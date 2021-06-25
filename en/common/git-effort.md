---
layout: default
title: "git effort"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-effort">
  <a href="/en/common/git-effort.html">git effort</a> <a href="#git-effort"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display how much activity a file has had, showing commits per file and "active days" i.e. total number of days that contributed to the file.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-effort>.

#### Display each file in the repository, showing commits and active days:
```shell
git effort
```
#### Display files modified by a specific number of commits or more, showing commits and active days:
```shell
git effort --above {{5}}
```
#### Display files modified by a specific author, showing commits and active days:
```shell
git effort -- --author="{{username}}"
```
#### Display files modified since a specific time/date, showing commits and active days:
```shell
git effort -- --since="{{last month}}"
```
#### Display only the specified files or directories, showing commits and active days:
```shell
git effort {{path/to/file_or_directory1 path/to/file_or_directory2 ...}}
```
#### Display all files in a specific directory, showing commits and active days:
```shell
git effort {{path/to/directory/*}}
```
{% endraw %}