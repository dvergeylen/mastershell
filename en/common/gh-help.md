---
layout: default
title: "gh help"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gh-help">
  <a href="/en/common/gh-help.html">gh help</a> <a href="#gh-help"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display help about the GitHub CLI command.
> More information: <https://cli.github.com/manual/gh_help>.

#### Display general help:
```shell
gh help
```
#### Display help for the `gh help` subcommand:
```shell
gh help --help
```
#### Display help about environment variables that can be used with `gh`:
```shell
gh help environment
```
#### Display a markdown reference of all `gh` commands:
```shell
gh help reference
```
#### Display help for a subcommand:
```shell
gh help {{subcommand}}
```
#### Display help for a subcommand action:
```shell
gh help {{pr}} {{create}}
```
{% endraw %}