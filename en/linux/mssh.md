---
layout: default
title: "mssh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mssh">
  <a href="/en/linux/mssh.html">mssh</a> <a href="#mssh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> GTK+ based SSH client for interacting with multiple SSH servers at once.

#### Open a new window and connect to multiple SSH servers:
```shell
mssh {{user@host1}} {{user@host2}} {{...}}
```
#### Open a new window and connect to a group of servers predefined in `~/.mssh_clusters`:
```shell
mssh --alias {{alias_name}}
```
{% endraw %}