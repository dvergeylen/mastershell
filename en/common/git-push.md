---
layout: default
title: "git push"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-push">
  <a href="/en/common/git-push.html">git push</a> <a href="#git-push"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Push commits to a remote repository.
> More information: <https://git-scm.com/docs/git-push>.

#### Send local changes in the current branch to its remote counterpart:
```shell
git push
```
#### Send local changes in a given branch to its remote counterpart:
```shell
git push {{remote_name}} {{local_branch}}
```
#### Publish the current branch to a remote repository, setting the remote branch name:
```shell
git push {{remote_name}} -u {{remote_branch}}
```
#### Send changes on all local branches to their counterparts in a given remote repository:
```shell
git push --all {{remote_name}}
```
#### Delete a branch in a remote repository:
```shell
git push {{remote_name}} --delete {{remote_branch}}
```
#### Remove remote branches that don't have a local counterpart:
```shell
git push --prune {{remote_name}}
```
#### Publish tags that aren't yet in the remote repository:
```shell
git push --tags
```
{% endraw %}