---
layout: default
title: "exa"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="exa">
  <a href="/en/common/exa.html">exa</a> <a href="#exa"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A modern replacement for `ls` (List directory contents).
> More information: <https://the.exa.website>.

#### List files one per line:
```shell
exa --oneline
```
#### List all files, including hidden files:
```shell
exa --all
```
#### Long format list (permissions, ownership, size and modification date) of all files:
```shell
exa --long --all
```
#### List files with the largest at the top:
```shell
exa --reverse --sort={{size}}
```
#### Display a tree of files, three levels deep:
```shell
exa --long --tree --level={{3}}
```
#### List files sorted by modification date (oldest first):
```shell
exa --long --sort={{modified}}
```
#### List files with their headers, icons, and Git statuses:
```shell
exa --long --header --icons --git
```
#### Don't list files mentioned in `.gitignore`:
```shell
exa --git-ignore
```
{% endraw %}