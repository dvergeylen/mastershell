---
layout: default
title: "git"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git">
  <a href="/en/common/git.html">git</a> <a href="#git"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Distributed version control system.
> More information: <https://git-scm.com/>.

#### Check the Git version:
```shell
git --version
```
#### Show general help:
```shell
git --help
```
#### Show help on a Git subcommand (like `commit`, `log`, etc.):
```shell
git help {{subcommand}}
```
#### Execute a Git subcommand:
```shell
git {{subcommand}}
```
#### Execute a Git subcommand on a custom repository root path:
```shell
git -C {{path/to/repo}} {{subcommand}}
```
#### Execute a Git subcommand with a given configuration set:
```shell
git -c '{{config.key}}={{value}}' {{subcommand}}
```
{% endraw %}