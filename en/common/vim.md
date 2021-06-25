---
layout: default
title: "vim"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vim">
  <a href="/en/common/vim.html">vim</a> <a href="#vim"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Vim (Vi IMproved), a command-line text editor, provides several modes for different kinds of text manipulation.
> Pressing `i` enters edit mode. `<Esc>` goes back to normal mode, which doesn't allow regular text insertion.
> More information: <https://www.vim.org>.

#### Open a file:
```shell
vim {{path/to/file}}
```
#### View Vim's help manual:
```shell
:help<Enter>
```
#### Save and Quit:
```shell
:wq<Enter>
```
#### Open a file at a specified line number:
```shell
vim +{{line_number}} {{path/to/file}}
```
#### Undo the last operation:
```shell
u
```
#### Search for a pattern in the file (press `n`/`N` to go to next/previous match):
```shell
/{{search_pattern}}<Enter>
```
#### Perform a regular expression substitution in the whole file:
```shell
:%s/{{regular_expression}}/{{replacement}}/g<Enter>
```
#### Display the line numbers:
```shell
:set nu<Enter>
```
{% endraw %}