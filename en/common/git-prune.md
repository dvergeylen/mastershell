---
layout: default
title: "git prune"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-prune">
  <a href="/en/common/git-prune.html">git prune</a> <a href="#git-prune"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Git command for pruning all unreachable objects from the object database.
> This command is often not used directly but as an internal command that is used by Git gc.
> More information: <https://git-scm.com/docs/git-prune>.

#### Report what would be removed by Git prune without removing it:
```shell
git prune --dry-run
```
#### Prune unreachable objects and display what has been pruned to stdout:
```shell
git prune --verbose
```
#### Prune unreachable objects while showing progress:
```shell
git prune --progress
```
{% endraw %}