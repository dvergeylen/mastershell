---
layout: default
title: "git-imerge"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-imerge">
  <a href="/en/common/git-imerge.html">git-imerge</a> <a href="#git-imerge"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Perform a merge or rebase between two Git branches incrementally.
> Conflicts between branches are tracked down to pairs of individual commits, to simplify conflict resolution.
> More information: <https://github.com/mhagger/git-imerge>.

#### Start imerge-based rebase (checkout the branch to be rebased, first):
```shell
git imerge rebase {{branch_to_rebase_onto}}
```
#### Start imerge-based merge (checkout the branch to merge into, first):
```shell
git imerge merge {{branch_to_be_merged}}
```
#### Show ASCII diagram of in-progress merge or rebase:
```shell
git imerge diagram
```
#### Continue imerge operation after resolving conflicts (`git add` the conflicted files, first):
```shell
git imerge continue --no-edit
```
#### Wrap up imerge operation, after all conflicts are resolved:
```shell
git imerge finish
```
#### Abort imerge operation, and return to the previous branch:
```shell
git-imerge remove && git checkout {{previous_branch}}
```
{% endraw %}