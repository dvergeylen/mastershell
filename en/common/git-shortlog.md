---
layout: default
title: "git shortlog"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-shortlog">
  <a href="/en/common/git-shortlog.html">git shortlog</a> <a href="#git-shortlog"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Summarizes the `git log` output.
> More information: <https://git-scm.com/docs/git-shortlog>.

#### View a summary of all the commits made, grouped alphabetically by author name:
```shell
git shortlog
```
#### View a summary of all the commits made, sorted by the number of commits made:
```shell
git shortlog -n
```
#### View a summary of all the commits made, grouped by the committer identities (name and email):
```shell
git shortlog -c
```
#### View a summary of the last 5 commits (i.e. specify a revision range):
```shell
git shortlog HEAD~{{5}}..HEAD
```
#### View all users, emails and the number of commits in the current branch:
```shell
git shortlog -sne
```
#### View all users, emails and the number of commits in all branches:
```shell
git shortlog -sne --all
```
{% endraw %}