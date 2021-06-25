---
layout: default
title: "git bundle"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-bundle">
  <a href="/en/common/git-bundle.html">git bundle</a> <a href="#git-bundle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Package objects and references into an archive.
> More information: <https://git-scm.com/docs/git-bundle>.

#### Create a bundle file that contains all objects and references of a specific branch:
```shell
git bundle create {{path/to/file.bundle}} {{branch_name}}
```
#### Create a bundle file of all branches:
```shell
git bundle create {{path/to/file.bundle}} --all
```
#### Create a bundle file of the last 5 commits of the current branch:
```shell
git bundle create {{path/to/file.bundle}} -{{5}} {{HEAD}}
```
#### Create a bundle file of the latest 7 days:
```shell
git bundle create {{path/to/file.bundle}} --since={{7.days}} {{HEAD}}
```
#### Verify that a bundle file is valid and can be applied to the current repository:
```shell
git bundle verify {{path/to/file.bundle}}
```
#### Print to the standard output the list of references contained in a bundle:
```shell
git bundle unbundle {{path/to/file.bundle}}
```
#### Unbundle a specific branch from a bundle file into the current repository:
```shell
git pull {{path/to/file.bundle}} {{branch_name}}
```
{% endraw %}