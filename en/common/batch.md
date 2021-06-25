---
layout: default
title: "batch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="batch">
  <a href="/en/common/batch.html">batch</a> <a href="#batch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Execute commands at a later time when the system load levels permit.
> Service atd (or atrun) should be running for the actual executions.
> More information: <https://man.archlinux.org/man/at.1>.

#### Execute commands from standard input (press `Ctrl + D` when done):
```shell
batch
```
#### Execute a command from standard input:
```shell
echo "{{./make_db_backup.sh}}" | batch
```
#### Execute commands from a given file:
```shell
batch -f {{path/to/file}}
```
{% endraw %}