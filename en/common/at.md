---
layout: default
title: "at"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="at">
  <a href="/en/common/at.html">at</a> <a href="#at"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Execute commands once at a later time.
> Service atd (or atrun) should be running for the actual executions.
> More information: <https://man.archlinux.org/man/at.1>.

#### Execute commands from standard input in 5 minutes (press `Ctrl + D` when done):
```shell
at now + 5 minutes
```
#### Execute a command from standard input at 10:00 AM today:
```shell
echo "{{./make_db_backup.sh}}" | at 1000
```
#### Execute commands from a given file next Tuesday:
```shell
at -f {{path/to/file}} 9:30 PM Tue
```
{% endraw %}