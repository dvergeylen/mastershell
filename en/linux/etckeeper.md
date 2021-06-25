---
layout: default
title: "etckeeper"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="etckeeper">
  <a href="/en/linux/etckeeper.html">etckeeper</a> <a href="#etckeeper"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Track system configuration files in Git.
> More information: <http://etckeeper.branchable.com/>.

#### Set up a Git repo and perform various setup tasks (run from `/etc`):
```shell
sudo etckeeper init
```
#### Commit all changes in `/etc`:
```shell
sudo etckeeper commit {{message}}
```
#### Run arbitrary Git commands:
```shell
sudo etckeeper vcs {{status}}
```
#### Check if there are uncommitted changes (only returns an exit code):
```shell
sudo etckeeper unclean
```
#### Destroy existing repo and stop tracking changes:
```shell
sudo etckeeper uninit
```
{% endraw %}