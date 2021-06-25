---
layout: default
title: "kill"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kill">
  <a href="/en/common/kill.html">kill</a> <a href="#kill"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sends a signal to a process, usually related to stopping the process.
> All signals except for SIGKILL and SIGSTOP can be intercepted by the process to perform a clean exit.

#### Terminate a program using the default SIGTERM (terminate) signal:
```shell
kill {{process_id}}
```
#### List available signal names (to be used without the `SIG` prefix):
```shell
kill -l
```
#### Terminate a background job:
```shell
kill %{{job_id}}
```
#### Terminate a program using the SIGHUP (hang up) signal. Many daemons will reload instead of terminating:
```shell
kill -{{1|HUP}} {{process_id}}
```
#### Terminate a program using the SIGINT (interrupt) signal. This is typically initiated by the user pressing `Ctrl + C`:
```shell
kill -{{2|INT}} {{process_id}}
```
#### Signal the operating system to immediately terminate a program (which gets no chance to capture the signal):
```shell
kill -{{9|KILL}} {{process_id}}
```
#### Signal the operating system to pause a program until a SIGCONT ("continue") signal is received:
```shell
kill -{{17|STOP}} {{process_id}}
```
#### Send a `SIGUSR1` signal to all processes with the given GID (group id):
```shell
kill -{{SIGUSR1}} -{{group_id}}
```
{% endraw %}