---
layout: default
title: "git range-diff"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-range-diff">
  <a href="/en/common/git-range-diff.html">git range-diff</a> <a href="#git-range-diff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compare two commit ranges (e.g. two versions of a branch).
> More information: <https://git-scm.com/docs/git-range-diff>.

#### Diff the changes of two individual commits:
```shell
git range-diff {{commit_1}}^! {{commit_2}}^!
```
#### Diff the changes of ours and theirs from their common ancestor, e.g. after an interactive rebase:
```shell
git range-diff {{theirs}}...{{ours}}
```
#### Diff the changes of two commit ranges, e.g. to check whether conflicts have been resolved appropriately when rebasing commits from `base1` to `base2`:
```shell
git range-diff {{base1}}..{{rev1}} {{base2}}..{{rev2}}
```
{% endraw %}