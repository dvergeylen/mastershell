---
layout: default
title: "git status"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-status">
  <a href="/en/common/git-status.html">git status</a> <a href="#git-status"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show the changes to files in a Git repository.
> Lists changed, added and deleted files compared to the currently checked-out commit.
> More information: <https://git-scm.com/docs/git-status>.

#### Show changed files which are not yet added for commit:
```shell
git status
```
#### Give output in [s]hort format:
```shell
git status -s
```
#### Don't show untracked files in the output:
```shell
git status --untracked-files=no
```
#### Show output in [s]hort format along with [b]ranch info:
```shell
git status -sb
```
{% endraw %}