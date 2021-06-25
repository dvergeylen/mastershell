---
layout: default
title: "tree"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tree">
  <a href="/en/windows/tree.html">tree</a> <a href="#tree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display a graphical tree of the directory structure for a path.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/tree>.

#### Display the tree for the current directory:
```shell
tree
```
#### Display the tree for a specific directory:
```shell
tree {{path/to/directory}}
```
#### Display the tree for a directory including files:
```shell
tree {{path/to/directory}} /f
```
#### Display the tree using ASCII characters instead of extended characters:
```shell
tree {{path/to/directory}} /a
```
{% endraw %}