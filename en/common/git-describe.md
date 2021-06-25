---
layout: default
title: "git describe"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-describe">
  <a href="/en/common/git-describe.html">git describe</a> <a href="#git-describe"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Give an object a human readable name based on an available ref.
> More information: <https://git-scm.com/docs/git-describe>.

#### Create a unique name for the current commit (the name contains the most recent annotated tag, the number of additional commits, and the abbreviated commit hash):
```shell
git describe
```
#### Create a name with 4 digits for the abbreviated commit hash:
```shell
git describe --abbrev={{4}}
```
#### Generate a name with the tag reference path:
```shell
git describe --all
```
#### Describe a Git tag:
```shell
git describe {{v1.0.0}}
```
#### Create a name for the last commit of a given branch:
```shell
git describe {{branch_name}}
```
{% endraw %}