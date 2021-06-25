---
layout: default
title: "git show-index"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-show-index">
  <a href="/en/common/git-show-index.html">git show-index</a> <a href="#git-show-index"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show the packed archive index of a Git repository.
> More information: <https://git-scm.com/docs/git-show-index>.

#### Read an IDX file for a Git packfile and dump its contents to stdout:
```shell
git show-index {{path/to/file.idx}}
```
#### Specify the hash algorithm for the index file (experimental):
```shell
git show-index --object-format={{sha1|sha256}} {{path/to/file}}
```
{% endraw %}