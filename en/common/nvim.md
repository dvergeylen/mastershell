---
layout: default
title: "nvim"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nvim">
  <a href="/en/common/nvim.html">nvim</a> <a href="#nvim"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Neovim, a programmer's text editor based on Vim, provides several modes for different kinds of text manipulation.
> Pressing `i` enters edit mode. `<Esc>` goes back to normal mode, which doesn't allow regular text insertion.
> More information: <https://neovim.io>.

#### Open a file:
```shell
nvim {{file}}
```
#### Enter text editing mode (insert mode):
```shell
<Esc>i
```
#### Copy ("yank") or cut ("delete") the current line (paste it with `P`):
```shell
<Esc>{{yy|dd}}
```
#### Undo the last operation:
```shell
<Esc>u
```
#### Search for a pattern in the file (press `n`/`N` to go to next/previous match):
```shell
<Esc>/{{search_pattern}}<Enter>
```
#### Perform a regular expression substitution in the whole file:
```shell
<Esc>:%s/{{regular_expression}}/{{replacement}}/g<Enter>
```
#### Save (write) the file, and quit:
```shell
<Esc>:wq<Enter>
```
#### Quit without saving:
```shell
<Esc>:q!<Enter>
```
{% endraw %}