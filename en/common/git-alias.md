---
layout: default
title: "git alias"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-alias">
  <a href="/en/common/git-alias.html">git alias</a> <a href="#git-alias"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create shortcuts for Git commands.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-alias>.

#### List all aliases:
```shell
git alias
```
#### Create a new alias:
```shell
git alias "{{name}}" "{{command}}"
```
#### Search for an existing alias:
```shell
git alias ^{{name}}
```
{% endraw %}