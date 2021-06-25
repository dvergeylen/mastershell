---
layout: default
title: "chattr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chattr">
  <a href="/en/linux/chattr.html">chattr</a> <a href="#chattr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change attributes of files or directories.

#### Make a file or directory immutable to changes and deletion, even by superuser:
```shell
chattr +i {{path/to/file_or_directory}}
```
#### Make a file or directory mutable:
```shell
chattr -i {{path/to/file_or_directory}}
```
#### Recursively make an entire directory and contents immutable:
```shell
chattr -R +i {{path/to/directory}}
```
{% endraw %}