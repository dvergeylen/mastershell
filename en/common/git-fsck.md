---
layout: default
title: "git fsck"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-fsck">
  <a href="/en/common/git-fsck.html">git fsck</a> <a href="#git-fsck"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verify the validity and connectivity of nodes in a Git repository index.
> Does not make any modifications. See `git gc` for cleaning up dangling blobs.
> More information: <https://git-scm.com/docs/git-fsck>.

#### Check the current repository:
```shell
git fsck
```
#### List all tags found:
```shell
git fsck --tags
```
#### List all root nodes found:
```shell
git fsck --root
```
{% endraw %}