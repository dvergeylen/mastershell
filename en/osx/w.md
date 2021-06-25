---
layout: default
title: "w"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="w">
  <a href="/en/osx/w.html">w</a> <a href="#w"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show who is logged on and what they are doing.
> Print user login, TTY, remote host, login time, idle time, current process.

#### Show logged-in users info:
```shell
w
```
#### Show logged-in users info without a header:
```shell
w -h
```
#### Show info about logged-in users, sorted by their idle time:
```shell
w -i
```
{% endraw %}