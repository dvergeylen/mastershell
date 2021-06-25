---
layout: default
title: "git obliterate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-obliterate">
  <a href="/en/common/git-obliterate.html">git obliterate</a> <a href="#git-obliterate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Delete specific files and erase their history from a Git repository.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-obliterate>.

#### Erase the existence of specific files:
```shell
git obliterate {{file_1 file_2 ...}}
```
#### Erase the existence of specific files between 2 commits:
```shell
git obliterate {{file_1 file_2 ...}} -- {{commit_hash_1}}..{{commit_hash_2}}
```
{% endraw %}