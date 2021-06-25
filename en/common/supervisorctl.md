---
layout: default
title: "supervisorctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="supervisorctl">
  <a href="/en/common/supervisorctl.html">supervisorctl</a> <a href="#supervisorctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Supervisor is a client/server system that allows its users to control a number of processes on UNIX-like operating systems.
> Supervisorctl is the command-line client piece of the supervisor which provides a shell-like interface.
> More information: <http://supervisord.org>.

#### Start/stop/restart a process:
```shell
supervisorctl {{start|stop|restart}} {{process_name}}
```
#### Start/stop/restart all processes in a group:
```shell
supervisorctl {{start|stop|restart}} {{group_name}}:*
```
#### Show last 100 **bytes** of process stderr:
```shell
supervisorctl tail -100 {{process_name}} stderr
```
#### Keep displaying stdout of a process:
```shell
supervisorctl tail -f {{process_name}} stdout
```
#### Reload process config file to add/remove processes as necessary:
```shell
supervisorctl update
```
{% endraw %}