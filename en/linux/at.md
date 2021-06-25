---
layout: default
title: "at"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="at">
  <a href="/en/linux/at.html">at</a> <a href="#at"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Executes commands at a specified time.
> More information: <https://man.archlinux.org/man/at.1>.

#### Open an `at` prompt to create a new set of scheduled commands, press `Ctrl + D` to save and exit:
```shell
at {{hh:mm}}
```
#### Execute the commands and email the result using a local mailing program such as sendmail:
```shell
at {{hh:mm}} -m
```
#### Execute a script at the given time:
```shell
at {{hh:mm}} -f {{path/to/file}}
```
#### Display a system notification at 11pm on February 18th:
```shell
echo "notify-send '{{Wake up!}}'" | at {{11pm}} {{Feb 18}}
```
{% endraw %}