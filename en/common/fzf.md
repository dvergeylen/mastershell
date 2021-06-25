---
layout: default
title: "fzf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fzf">
  <a href="/en/common/fzf.html">fzf</a> <a href="#fzf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line fuzzy finder.
> Similar to `sk`.
> More information: <https://github.com/junegunn/fzf>.

#### Start fzf on all files in the specified directory:
```shell
find {{path/to/directory}} -type f | fzf
```
#### Start fzf for running processes:
```shell
ps aux | fzf
```
#### Select multiple files with `Shift + Tab` and write to a file:
```shell
find {{path/to/directory}} -type f | fzf --multi > {{filename}}
```
#### Start fzf with a specified query:
```shell
fzf --query "{{query}}"
```
#### Start fzf on entries that start with core and end with either go, rb, or py:
```shell
fzf --query "^core go$ | rb$ | py$"
```
#### Start fzf on entries that not match pyc and match exactly travis:
```shell
fzf --query "!pyc 'travis"
```
{% endraw %}