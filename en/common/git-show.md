---
layout: default
title: "git show"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-show">
  <a href="/en/common/git-show.html">git show</a> <a href="#git-show"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show various types of Git objects (commits, tags, etc.).
> More information: <https://git-scm.com/docs/git-show>.

#### Show information about the latest commit (hash, message, changes, and other metadata):
```shell
git show
```
#### Show information about a given commit:
```shell
git show {{commit}}
```
#### Show information about the commit associated with a given tag:
```shell
git show {{tag}}
```
#### Show information about the 3rd commit from the HEAD of a branch:
```shell
git show {{branch}}~{{3}}
```
#### Show a commit's message in a single line, suppressing the diff output:
```shell
git show --oneline -s {{commit}}
```
#### Show only statistics (added/removed characters) about the changed files:
```shell
git show --stat {{commit}}
```
#### Show only the list of added, renamed or deleted files:
```shell
git show --summary {{commit}}
```
#### Show the contents of a file as it was at a given revision (e.g. branch, tag or commit):
```shell
git show {{revision}}:{{path/to/file}}
```
{% endraw %}