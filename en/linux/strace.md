---
layout: default
title: "strace"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="strace">
  <a href="/en/linux/strace.html">strace</a> <a href="#strace"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Troubleshooting tool for tracing system calls.

#### Start tracing a specific process by its PID:
```shell
strace -p {{pid}}
```
#### Trace a process and filter output by system call:
```shell
strace -p {{pid}} -e {{system_call_name}}
```
#### Count time, calls, and errors for each system call and report a summary on program exit:
```shell
strace -p {{pid}} -c
```
#### Show the time spent in every system call:
```shell
strace -p {{pid}} -T
```
#### Start tracing a program by executing it:
```shell
strace {{program}}
```
#### Start tracing file operations of a program:
```shell
strace -e trace=file {{program}}
```
{% endraw %}