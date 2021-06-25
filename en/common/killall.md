---
layout: default
title: "killall"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="killall">
  <a href="/en/common/killall.html">killall</a> <a href="#killall"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Send kill signal to all instances of a process by name (must be exact name).
> All signals except SIGKILL and SIGSTOP can be intercepted by the process, allowing a clean exit.

#### Terminate a process using the default SIGTERM (terminate) signal:
```shell
killall {{process_name}}
```
#### List available signal names (to be used without the 'SIG' prefix):
```shell
killall --list
```
#### Interactively ask for confirmation before termination:
```shell
killall -i {{process_name}}
```
#### Terminate a process using the SIGINT (interrupt) signal, which is the same signal sent by pressing `Ctrl + C`:
```shell
killall -INT {{process_name}}
```
#### Force kill a process:
```shell
killall -KILL {{process_name}}
```
{% endraw %}