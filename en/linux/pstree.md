---
layout: default
title: "pstree"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pstree">
  <a href="/en/linux/pstree.html">pstree</a> <a href="#pstree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A convenient tool to show running processes as a tree.

#### Display a tree of processes:
```shell
pstree
```
#### Display a tree of processes with PIDs:
```shell
pstree -p
```
#### Display all process trees rooted at processes owned by specified user:
```shell
pstree {{user}}
```
{% endraw %}