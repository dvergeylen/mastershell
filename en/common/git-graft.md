---
layout: default
title: "git graft"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-graft">
  <a href="/en/common/git-graft.html">git graft</a> <a href="#git-graft"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Merge commits from a specific branch into another branch and delete the source branch.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-graft>.

#### Merge all commits not present on the target branch from the source branch to target branch, and delete the source branch:
```shell
git graft {{source_branch}} {{target_branch}}
```
{% endraw %}