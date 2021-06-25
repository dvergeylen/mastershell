---
layout: default
title: "hg pull"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hg-pull">
  <a href="/en/common/hg-pull.html">hg pull</a> <a href="#hg-pull"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pull changes from a specified repository to the local repository.
> More information: <https://www.mercurial-scm.org/doc/hg.1.html#pull>.

#### Pull from the "default" source path:
```shell
hg pull
```
#### Pull from a specified source repository:
```shell
hg pull {{path/to/source_repository}}
```
#### Update the local repository to the head of the remote:
```shell
hg pull --update
```
#### Pull changes even when the remote repository is unrelated:
```shell
hg pull --force
```
#### Specify a specific revision changeset to pull up to:
```shell
hg pull --rev {{revision}}
```
#### Specify a specific branch to pull:
```shell
hg pull --branch {{branch}}
```
#### Specify a specific bookmark to pull:
```shell
hg pull --bookmark {{bookmark}}
```
{% endraw %}