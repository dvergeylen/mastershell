---
layout: default
title: "git rev-parse"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-rev-parse">
  <a href="/en/common/git-rev-parse.html">git rev-parse</a> <a href="#git-rev-parse"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display metadata related to specific revisions.
> More information: <https://git-scm.com/docs/git-rev-parse>.

#### Get the commit hash of a branch:
```shell
git rev-parse {{branch_name}}
```
#### Get the current branch name:
```shell
git rev-parse --abbrev-ref {{HEAD}}
```
#### Get the absolute path to the root directory:
```shell
git rev-parse --show-toplevel
```
{% endraw %}