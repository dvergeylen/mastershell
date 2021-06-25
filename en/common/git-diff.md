---
layout: default
title: "git diff"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-diff">
  <a href="/en/common/git-diff.html">git diff</a> <a href="#git-diff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show changes to tracked files.
> More information: <https://git-scm.com/docs/git-diff>.

#### Show unstaged, uncommitted changes:
```shell
git diff
```
#### Show all uncommitted changes (including staged ones):
```shell
git diff HEAD
```
#### Show only staged (added, but not yet committed) changes:
```shell
git diff --staged
```
#### Show changes from all commits since a given date/time (a date expression, e.g. "1 week 2 days" or an ISO date):
```shell
git diff 'HEAD@{3 months|weeks|days|hours|seconds ago}'
```
#### Show only names of changed files since a given commit:
```shell
git diff --name-only {{commit}}
```
#### Output a summary of file creations, renames and mode changes since a given commit:
```shell
git diff --summary {{commit}}
```
#### Compare a single file between two branches or commits:
```shell
git diff {{branch_1}}..{{branch_2}} [--] {{path/to/file}}
```
#### Compare different files from the current branch to other branch:
```shell
git diff {{branch}}:{{path/to/file2}} {{path/to/file}}
```
{% endraw %}