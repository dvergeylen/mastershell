---
layout: default
title: "write"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="write">
  <a href="/en/common/write.html">write</a> <a href="#write"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Write a message on the terminal of a specified logged in user (ctrl-C to stop writing messages).
> Use the `who` command to find out all terminal_ids of all active users active on the system. See also `mesg`.

#### Send a message to a given user on a given terminal id:
```shell
write {{username}} {{terminal_id}}
```
#### Send message to "testuser" on terminal `/dev/tty/5`:
```shell
write {{testuser}} {{tty/5}}
```
#### Send message to "johndoe" on pseudo terminal `/dev/pts/5`:
```shell
write {{johndoe}} {{pts/5}}
```
{% endraw %}