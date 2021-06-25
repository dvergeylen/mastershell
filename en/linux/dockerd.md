---
layout: default
title: "dockerd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dockerd">
  <a href="/en/linux/dockerd.html">dockerd</a> <a href="#dockerd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A persistent process to start and manage docker containers.
> More information: <https://docs.docker.com/engine/reference/commandline/dockerd/>.

#### Run docker daemon:
```shell
dockerd
```
#### Run docker daemon and config it to listen to specific sockets(unix,tcp):
```shell
dockerd --host unix://{{path/to/tmp.sock}} --host tcp://{{ip}}
```
#### Run with specific daemon PID file:
```shell
dockerd --pidfile {{path/to/pid_file}}
```
#### Run in debug mode:
```shell
dockerd --debug
```
#### Run and set a specific log level:
```shell
dockerd --log-level={{debug|info|warn|error|fatal}}
```
{% endraw %}