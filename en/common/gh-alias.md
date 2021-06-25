---
layout: default
title: "gh alias"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gh-alias">
  <a href="/en/common/gh-alias.html">gh alias</a> <a href="#gh-alias"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage GitHub CLI command aliases from the command-line.
> More information: <https://cli.github.com/manual/gh_alias>.

#### Display the subcommand help:
```shell
gh alias
```
#### List all of the aliases `gh` is configured to use:
```shell
gh alias list
```
#### Create a `gh` subcommand alias:
```shell
gh alias set {{pv}} '{{pr view}}'
```
#### Set a shell command as a `gh` subcommand:
```shell
gh alias set --shell {{alias_name}} {{command}}
```
#### Delete a command shortcut:
```shell
gh alias delete {{alias_name}}
```
{% endraw %}