---
layout: default
title: "git ls-tree"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-ls-tree">
  <a href="/en/common/git-ls-tree.html">git ls-tree</a> <a href="#git-ls-tree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List the contents of a tree object.
> More information: <https://git-scm.com/docs/git-ls-tree>.

#### List the contents of the tree on a branch:
```shell
git ls-tree {{branch_name}}
```
#### List the contents of the tree on a commit, recursing into subtrees:
```shell
git ls-tree -r {{commit_hash}}
```
#### List only the filenames of the tree on a commit:
```shell
git ls-tree --name-only {{commit_hash}}
```
{% endraw %}