---
layout: default
title: "kak"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kak">
  <a href="/en/common/kak.html">kak</a> <a href="#kak"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kakoune is a mode-based code editor implementing the "multiple selections" paradigm.
> Data can be selected and simultaneously edited in different locations, using multiple selections; users can also connect to the same session for collaborative editing.
> More information: <https://kakoune.org>.

#### Open a file and enter normal mode, to execute commands:
```shell
kak {{path/to/file}}
```
#### Enter insert mode from normal mode, to write text into the file:
```shell
i
```
#### Escape insert mode, to go back to normal mode:
```shell
<Escape>
```
#### Replace all instances of "foo" in the current file with "bar":
```shell
%s{{foo}}<Enter>c{{bar}}<Escape>
```
#### Un-select all secondary selections, and keep only the main one:
```shell
<Space>
```
#### Search for numbers and select the first two:
```shell
/\d+<Enter>N
```
#### Insert the contents of a file:
```shell
!cat {{path/to/file}}<Enter>
```
#### Save the current file:
```shell
:w<Enter>
```
{% endraw %}