---
layout: default
title: "cd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cd">
  <a href="/en/windows/cd.html">cd</a> <a href="#cd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Displays the name of or changes the current working directory.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/cd>.

#### Go to a directory in the same drive:
```shell
cd {{path/to/directory}}
```
#### Display the name of the current directory:
```shell
cd
```
#### Go up to the parent of the current directory:
```shell
cd ..
```
#### Go to a directory in a different drive:
```shell
cd {{path/to/directory}} /d
```
{% endraw %}