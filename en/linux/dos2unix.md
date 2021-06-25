---
layout: default
title: "dos2unix"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dos2unix">
  <a href="/en/linux/dos2unix.html">dos2unix</a> <a href="#dos2unix"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change DOS-style line endings to Unix-style.
> Replaces CRLF with CR.

#### Change the line endings of a file:
```shell
dos2unix {{filename}}
```
#### Create a copy with Unix-style line endings:
```shell
dos2unix -n {{filename}} {{new_filename}}
```
{% endraw %}