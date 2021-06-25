---
layout: default
title: "git difftool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-difftool">
  <a href="/en/common/git-difftool.html">git difftool</a> <a href="#git-difftool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show file changes using external diff tools. Accepts the same options and arguments as `git diff`.
> See also: `git diff`.
> More information: <https://git-scm.com/docs/git-difftool>.

#### List available diff tools:
```shell
git difftool --tool-help
```
#### Set the default diff tool to meld:
```shell
git config --global diff.tool "{{meld}}"
```
#### Use the default diff tool to show staged changes:
```shell
git difftool --staged
```
#### Use a specific tool (opendiff) to show changes since a given commit:
```shell
git difftool --tool={{opendiff}} {{commit}}
```
{% endraw %}