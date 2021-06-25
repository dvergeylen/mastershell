---
layout: default
title: "cpulimit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cpulimit">
  <a href="/en/linux/cpulimit.html">cpulimit</a> <a href="#cpulimit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to throttle the CPU usage of other processes.
> More information: <http://cpulimit.sourceforge.net/>.

#### Limit an existing process with PID 1234 to only use 25% of the CPU:
```shell
cpulimit --pid {{1234}} --limit {{25%}}
```
#### Limit an existing program by its executable name:
```shell
cpulimit --exe {{program}} --limit {{25}}
```
#### Launch a given program and limit it to only use 50% of the CPU:
```shell
cpulimit --limit {{50}} -- {{program arg1 arg2 ...}}
```
#### Launch a program, limit its CPU usage to 50% and run cpulimit in the background:
```shell
cpulimit --limit {{50}} --background -- {{program}}
```
#### Kill its process if the program's CPU usage goes over 50%:
```shell
cpulimit --limit 50 --kill -- {{program}}
```
#### Throttle both it and its child processes so that none go about 25% CPU:
```shell
cpulimit --limit {{25}} --monitor-forks -- {{program}}
```
{% endraw %}