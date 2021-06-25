---
layout: default
title: "git fetch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-fetch">
  <a href="/en/common/git-fetch.html">git fetch</a> <a href="#git-fetch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Download objects and refs from a remote repository.
> More information: <https://git-scm.com/docs/git-fetch>.

#### Fetch the latest changes from the default remote upstream repository (if set):
```shell
git fetch
```
#### Fetch new branches from a specific remote upstream repository:
```shell
git fetch {{remote_name}}
```
#### Fetch the latest changes from all remote upstream repositories:
```shell
git fetch --all
```
#### Also fetch tags from the remote upstream repository:
```shell
git fetch --tags
```
#### Delete local references to remote branches that have been deleted upstream:
```shell
git fetch --prune
```
{% endraw %}