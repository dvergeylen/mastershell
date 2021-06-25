---
layout: default
title: "git commit-graph"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-commit-graph">
  <a href="/en/common/git-commit-graph.html">git commit-graph</a> <a href="#git-commit-graph"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Write and verify Git commit-graph files.
> More information: <https://git-scm.com/docs/git-commit-graph>.

#### Write a commit-graph file for the packed commits in the repository's local `.git` directory:
```shell
git commit-graph write
```
#### Write a commit-graph file containing all reachable commits:
```shell
git show-ref --hash | git commit-graph write --stdin-commits
```
#### Write a commit-graph file containing all commits in the current commit-graph file along with those reachable from `HEAD`:
```shell
git rev-parse {{HEAD}} | git commit-graph write --stdin-commits --append
```
{% endraw %}