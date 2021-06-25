---
layout: default
title: "git clean"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-clean">
  <a href="/en/common/git-clean.html">git clean</a> <a href="#git-clean"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove untracked files from the working tree.
> More information: <https://git-scm.com/docs/git-clean>.

#### Delete files that are not tracked by Git:
```shell
git clean
```
#### Interactively delete files that are not tracked by Git:
```shell
git clean -i
```
#### Show what files would be deleted without actually deleting them:
```shell
git clean --dry-run
```
#### Forcefully delete files that are not tracked by Git:
```shell
git clean -f
```
#### Forcefully delete directories that are not tracked by Git:
```shell
git clean -fd
```
#### Delete untracked files, including ignored files in `.gitignore` and `.git/info/exclude`:
```shell
git clean -x
```
{% endraw %}