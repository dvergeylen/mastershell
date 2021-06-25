---
layout: default
title: "git stage"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-stage">
  <a href="/en/common/git-stage.html">git stage</a> <a href="#git-stage"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Add file contents to the staging area.
> Synonym of `git add`.
> More information: <https://git-scm.com/docs/git-stage>.

#### Add a file to the index:
```shell
git stage {{path/to/file}}
```
#### Add all files (tracked and untracked):
```shell
git stage -A
```
#### Only add already tracked files:
```shell
git stage -u
```
#### Also add ignored files:
```shell
git stage -f
```
#### Interactively stage parts of files:
```shell
git stage -p
```
#### Interactively stage parts of a given file:
```shell
git stage -p {{path/to/file}}
```
#### Interactively stage a file:
```shell
git stage -i
```
{% endraw %}