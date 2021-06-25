---
layout: default
title: "unix2dos"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="unix2dos">
  <a href="/en/linux/unix2dos.html">unix2dos</a> <a href="#unix2dos"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change Unix-style line endings to DOS-style.
> Replaces CR with CRLF.

#### Change the line endings of a file:
```shell
unix2dos {{filename}}
```
#### Create a copy with DOS-style line endings:
```shell
unix2dos -n {{filename}} {{new_filename}}
```
{% endraw %}