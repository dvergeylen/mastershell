---
layout: default
title: "mac2unix"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mac2unix">
  <a href="/en/linux/mac2unix.html">mac2unix</a> <a href="#mac2unix"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change macOS-style line endings to Unix-style.
> Replaces LF with CR.

#### Change the line endings of a file:
```shell
mac2unix {{filename}}
```
#### Create a copy with Unix-style line endings:
```shell
mac2unix -n {{filename}} {{new_filename}}
```
{% endraw %}