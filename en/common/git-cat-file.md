---
layout: default
title: "git cat-file"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-cat-file">
  <a href="/en/common/git-cat-file.html">git cat-file</a> <a href="#git-cat-file"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Provide content or type and size information for Git repository objects.
> More information: <https://git-scm.com/docs/git-cat-file>.

#### Get the [s]ize of the HEAD commit in bytes:
```shell
git cat-file -s HEAD
```
#### Get the [t]ype (blob, tree, commit, tag) of a given Git object:
```shell
git cat-file -t {{8c442dc3}}
```
#### Pretty-[p]rint the contents of a given Git object based on its type:
```shell
git cat-file -p {{HEAD~2}}
```
{% endraw %}