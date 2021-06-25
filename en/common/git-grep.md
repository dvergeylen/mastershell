---
layout: default
title: "git-grep"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-grep">
  <a href="/en/common/git-grep.html">git-grep</a> <a href="#git-grep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Find strings inside files anywhere in a repository's history.
> Accepts a lot of the same flags as regular `grep`.
> More information: <https://git-scm.com/docs/git-grep>.

#### Search for a string in tracked files:
```shell
git grep {{search_string}}
```
#### Search for a string in files matching a pattern in tracked files:
```shell
git grep {{search_string}} -- {{file_glob_pattern}}
```
#### Search for a string in tracked files, including submodules:
```shell
git grep --recurse-submodules {{search_string}}
```
#### Search for a string at a specific point in history:
```shell
git grep {{search_string}} {{HEAD~2}}
```
#### Search for a string across all branches:
```shell
git grep {{search_string}} $(git rev-list --all)
```
{% endraw %}