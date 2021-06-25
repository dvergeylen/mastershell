---
layout: default
title: "git rebase"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-rebase">
  <a href="/en/common/git-rebase.html">git rebase</a> <a href="#git-rebase"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reapply commits from one branch on top of another branch.
> Commonly used to "move" an entire branch to another base, creating copies of the commits in the new location.
> More information: <https://git-scm.com/docs/git-rebase>.

#### Rebase the current branch on top of another specified branch:
```shell
git rebase {{new_base_branch}}
```
#### Start an interactive rebase, which allows the commits to be reordered, omitted, combined or modified:
```shell
git rebase -i {{target_base_branch_or_commit_hash}}
```
#### Continue a rebase that was interrupted by a merge failure, after editing conflicting files:
```shell
git rebase --continue
```
#### Continue a rebase that was paused due to merge conflicts, by skipping the conflicted commit:
```shell
git rebase --skip
```
#### Abort a rebase in progress (e.g. if it is interrupted by a merge conflict):
```shell
git rebase --abort
```
#### Move part of the current branch onto a new base, providing the old base to start from:
```shell
git rebase --onto {{new_base}} {{old_base}}
```
#### Reapply the last 5 commits in-place, stopping to allow them to be reordered, omitted, combined or modified:
```shell
git rebase -i {{HEAD~5}}
```
#### Auto-resolve any conflicts by favoring the working branch version (`theirs` keyword has reversed meaning in this case):
```shell
git rebase -X theirs {{branch_name}}
```
{% endraw %}