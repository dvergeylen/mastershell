---
layout: default
title: "git log"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-log">
  <a href="/en/common/git-log.html">git log</a> <a href="#git-log"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show a history of commits.
> More information: <https://git-scm.com/docs/git-log>.

#### Show the sequence of commits starting from the current one, in reverse chronological order of the Git repository in the current working directory:
```shell
git log
```
#### Show the history of a particular file or directory, including differences:
```shell
git log -p {{path/to/file_or_directory}}
```
#### Show an overview of which file(s) changed in each commit:
```shell
git log --stat
```
#### Show a graph of commits in the current branch using only the first line of each commit message:
```shell
git log --oneline --graph
```
#### Show a graph of all commits, tags and branches in the entire repo:
```shell
git log --oneline --decorate --all --graph
```
#### Show only commits whose messages include a given string (case-insensitively):
```shell
git log -i --grep {{search_string}}
```
#### Show the last N commits from a certain author:
```shell
git log -n {{number}} --author={{author}}
```
#### Show commits between two dates:
```shell
git log --before={{date}} --after={{date}}
```
{% endraw %}