---
layout: default
title: "dolt commit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dolt-commit">
  <a href="/en/common/dolt-commit.html">dolt commit</a> <a href="#dolt-commit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Commit staged changes to tables.
> More information: <https://docs.dolthub.com/interfaces/cli#dolt-commit>.

#### Commit all staged changes, opening the editor specified by `$EDITOR` to enter the commit message:
```shell
dolt commit
```
#### Commit all staged changes with the specified message:
```shell
dolt commit --message "{{commit_message}}"
```
#### Stage all unstaged changes to tables before committing:
```shell
dolt commit --all
```
#### Use the specified ISO 8601 commit date (defaults to current date and time):
```shell
dolt commit --date "{{2021-12-31T00:00:00}}"
```
#### Use the specified author for the commit:
```shell
dolt commit --author "{{author_name}} <{{author_email}}>"
```
#### Allow creating an empty commit, with no changes:
```shell
dolt commit --allow-empty
```
#### Ignore foreign key warnings:
```shell
dolt commit --force
```
{% endraw %}