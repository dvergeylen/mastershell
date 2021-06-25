---
layout: default
title: "lsof"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lsof">
  <a href="/en/common/lsof.html">lsof</a> <a href="#lsof"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lists open files and the corresponding processes.
> Note: Root privileges (or sudo) is required to list files opened by others.

#### Find the processes that have a given file open:
```shell
lsof {{path/to/file}}
```
#### Find the process that opened a local internet port:
```shell
lsof -i :{{port}}
```
#### Only output the process ID (PID):
```shell
lsof -t {{path/to/file}}
```
#### List files opened by the given user:
```shell
lsof -u {{username}}
```
#### List files opened by the given command or process:
```shell
lsof -c {{process_or_command_name}}
```
#### List files opened by a specific process, given its PID:
```shell
lsof -p {{PID}}
```
#### List open files in a directory:
```shell
lsof +D {{path/to/directory}}
```
#### Find the process that is listening on a local TCP port:
```shell
lsof -iTCP:{{port}} -sTCP:LISTEN
```
{% endraw %}