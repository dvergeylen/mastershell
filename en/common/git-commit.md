---
layout: default
title: "git commit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-commit">
  <a href="/en/common/git-commit.html">git commit</a> <a href="#git-commit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Commit files to the repository.
> More information: <https://git-scm.com/docs/git-commit>.

#### Commit staged files to the repository with a message:
```shell
git commit -m "{{message}}"
```
#### Commit staged files with a message read from a file:
```shell
git commit --file {{path/to/commit_message_file}}
```
#### Auto stage all modified files and commit with a message:
```shell
git commit -a -m "{{message}}"
```
#### Update the last commit by adding the currently staged changes, changing the commit's hash:
```shell
git commit --amend
```
#### Commit only specific (already staged) files:
```shell
git commit {{path/to/file1}} {{path/to/file2}}
```
#### Create a commit, even if there are no staged files:
```shell
git commit -m "{{message}}" --allow-empty
```
{% endraw %}