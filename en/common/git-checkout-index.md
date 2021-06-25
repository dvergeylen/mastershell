---
layout: default
title: "git checkout-index"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-checkout-index">
  <a href="/en/common/git-checkout-index.html">git checkout-index</a> <a href="#git-checkout-index"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copy files from the index to the working tree.
> More information: <https://git-scm.com/docs/git-checkout-index>.

#### Restore any files deleted since the last commit:
```shell
git checkout-index --all
```
#### Restore any files deleted or changed since the last commit:
```shell
git checkout-index --all --force
```
#### Restore any files changed since the last commit, ignoring any files that were deleted:
```shell
git checkout-index --all --force --no-create
```
#### Export a copy of the entire tree at the last commit to the specified directory (the trailing slash is important):
```shell
git checkout-index --all --force --prefix={{path/to/export_directory/}}
```
{% endraw %}