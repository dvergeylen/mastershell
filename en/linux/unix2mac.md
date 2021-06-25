---
layout: default
title: "unix2mac"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="unix2mac">
  <a href="/en/linux/unix2mac.html">unix2mac</a> <a href="#unix2mac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change Unix-style line endings to macOS-style.
> Replaces CR with LF.

#### Change the line endings of a file:
```shell
unix2mac {{filename}}
```
#### Create a copy with macOS-style line endings:
```shell
unix2mac -n {{filename}} {{new_filename}}
```
{% endraw %}