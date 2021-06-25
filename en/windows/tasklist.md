---
layout: default
title: "tasklist"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tasklist">
  <a href="/en/windows/tasklist.html">tasklist</a> <a href="#tasklist"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display a list of currently running processes on a local or remote machine.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/tasklist>.

#### Display currently running processes:
```shell
tasklist
```
#### Display running processes in a specified output format:
```shell
tasklist /fo {{table|list|csv}}
```
#### Display running processes using the specified `.exe` or `.dll` file name:
```shell
tasklist /m {{module_pattern}}
```
#### Display processes running on a remote machine:
```shell
tasklist /s {{remote_name}} /u {{username}} /p {{password}}
```
#### Display services using each process:
```shell
tasklist /svc
```
{% endraw %}