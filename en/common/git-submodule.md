---
layout: default
title: "git submodule"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-submodule">
  <a href="/en/common/git-submodule.html">git submodule</a> <a href="#git-submodule"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Inspects, updates and manages submodules.
> More information: <https://git-scm.com/docs/git-submodule>.

#### Install a repository's specified submodules:
```shell
git submodule update --init --recursive
```
#### Add a Git repository as a submodule:
```shell
git submodule add {{repository_url}}
```
#### Add a Git repository as a submodule at the specified directory:
```shell
git submodule add {{repository_url}} {{path/to/directory}}
```
#### Update every submodule to its latest commit:
```shell
git submodule foreach git pull
```
{% endraw %}