---
layout: default
title: "zile"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zile">
  <a href="/en/linux/zile.html">zile</a> <a href="#zile"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zile is a lightweight clone of the Emacs text editor.
> More information: <https://www.gnu.org/software/zile/>.

#### Start a buffer for temporary notes, which won't be saved:
```shell
zile
```
#### Open a file:
```shell
zile {{path/to/file}}
```
#### Save a file:
```shell
Ctrl + X, Ctrl + S
```
#### Quit:
```shell
Ctrl + X, Ctrl + C
```
#### Open a file at a specified line number:
```shell
zile +{{line_number}} {{path/to/file}}
```
#### Undo changes:
```shell
Ctrl + X, U
```
{% endraw %}