---
layout: default
title: "git show-branch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-show-branch">
  <a href="/en/common/git-show-branch.html">git show-branch</a> <a href="#git-show-branch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show branches and their commits.
> More information: <https://git-scm.com/docs/git-show-branch>.

#### Show a summary of the latest commit on a branch:
```shell
git show-branch {{branch_name|ref|commit}}
```
#### Compare commits in the history of multiple commits or branches:
```shell
git show-branch {{branch_name|ref|commit}}
```
#### Compare all remote tracking branches:
```shell
git show-branch --remotes
```
#### Compare both local and remote tracking branches:
```shell
git show-branch --all
```
#### List the latest commits in all branches:
```shell
git show-branch --all --list
```
#### Compare a given branch with the current branch:
```shell
git show-branch --current {{commit|branch_name|ref}}
```
#### Display the commit name instead of the relative name:
```shell
git show-branch --sha1-name --current {{current|branch_name|ref}}
```
#### Keep going a given number of commits past the common ancestor:
```shell
git show-branch --more {{5}} {{commit|branch_name|ref}} {{commit|branch_name|ref}} {{...}}
```
{% endraw %}