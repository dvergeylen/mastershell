---
layout: default
title: "autojump"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="autojump">
  <a href="/en/common/autojump.html">autojump</a> <a href="#autojump"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Quickly jump among the directories you visit the most.
> Aliases like j or jc are provided for even less typing.
> More information: <https://github.com/wting/autojump>.

#### Jump to a directory that contains the given pattern:
```shell
j {{pattern}}
```
#### Jump to a sub-directory (child) of the current directory that contains the given pattern:
```shell
jc {{pattern}}
```
#### Open a directory that contains the given pattern in the operating system file manager:
```shell
jo {{pattern}}
```
#### Remove non-existing directories from the autojump database:
```shell
j --purge
```
#### Show the entries in the autojump database:
```shell
j -s
```
{% endraw %}