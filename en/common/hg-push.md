---
layout: default
title: "hg push"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hg-push">
  <a href="/en/common/hg-push.html">hg push</a> <a href="#hg-push"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Push changes from the local repository to a specified destination.
> More information: <https://www.mercurial-scm.org/doc/hg.1.html#push>.

#### Push changes to the "default" remote path:
```shell
hg push
```
#### Push changes to a specified remote repository:
```shell
hg push {{path/to/destination_repository}}
```
#### Push a new branch if it does not exist (disabled by default):
```shell
hg push --new-branch
```
#### Specify a specific revision changeset to push:
```shell
hg push --rev {{revision}}
```
#### Specify a specific branch to push:
```shell
hg push --branch {{branch}}
```
#### Specify a specific bookmark to push:
```shell
hg push --bookmark {{bookmark}}
```
{% endraw %}