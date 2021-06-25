---
layout: default
title: "addpart"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="addpart">
  <a href="/en/linux/addpart.html">addpart</a> <a href="#addpart"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tells the Linux kernel about the existence of the specified partition.
> The command is a simple wrapper around the `add partition` ioctl.
> More information: <https://manned.org/addpart>.

#### Tell the kernel about the existence of the specified partition:
```shell
addpart {{device}} {{partition}} {{start}} {{length}}
```
{% endraw %}