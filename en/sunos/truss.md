---
layout: default
title: "truss"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="truss">
  <a href="/en/sunos/truss.html">truss</a> <a href="#truss"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Troubleshooting tool for tracing system calls.
> SunOS equivalent of strace.
> More information: <https://www.unix.com/man-page/linux/1/truss>.

#### Start tracing a program by executing it, following all child processes:
```shell
truss -f {{program}}
```
#### Start tracing a specific process by its PID:
```shell
truss -p {{pid}}
```
#### Start tracing a program by executing it, showing arguments and environment variables:
```shell
truss -a -e {{program}}
```
#### Count time, calls, and errors for each system call and report a summary on program exit:
```shell
truss -c -p {{pid}}
```
#### Trace a process filtering output by system call:
```shell
truss -p {{pid}} -t {{system_call_name}}
```
{% endraw %}