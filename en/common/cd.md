---
layout: default
title: "cd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cd">
  <a href="/en/common/cd.html">cd</a> <a href="#cd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change the current working directory.
> More information: <https://man.archlinux.org/man/cd.n>.

#### Go to the given directory:
```shell
cd {{path/to/directory}}
```
#### Go to home directory of current user:
```shell
cd
```
#### Go up to the parent of the current directory:
```shell
cd ..
```
#### Go to the previously chosen directory:
```shell
cd -
```
{% endraw %}