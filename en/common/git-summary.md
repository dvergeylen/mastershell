---
layout: default
title: "git summary"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-summary">
  <a href="/en/common/git-summary.html">git summary</a> <a href="#git-summary"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information about a Git repository.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-summary>.

#### Display data about a Git repository:
```shell
git summary
```
#### Display data about a Git repository since a commit-ish:
```shell
git summary {{commit|branch_name|tag_name}}
```
#### Display data about a Git repository, merging committers using different emails into 1 statistic for each author:
```shell
git summary --dedup-by-email
```
#### Display data about a Git repository, showing the number of lines modified by each contributer:
```shell
git summary --line
```
{% endraw %}