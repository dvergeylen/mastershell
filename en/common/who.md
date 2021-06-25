---
layout: default
title: "who"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="who">
  <a href="/en/common/who.html">who</a> <a href="#who"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display who is logged in and related data (processes, boot time).
> More information: <https://www.gnu.org/software/coreutils/who>.

#### Display the username, line, and time of all currently logged-in sessions:
```shell
who
```
#### Display information only for the current terminal session:
```shell
who am i
```
#### Display all available information:
```shell
who -a
```
#### Display all available information with table headers:
```shell
who -a -H
```
{% endraw %}