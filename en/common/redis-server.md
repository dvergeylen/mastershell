---
layout: default
title: "redis-server"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="redis-server">
  <a href="/en/common/redis-server.html">redis-server</a> <a href="#redis-server"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Persistent key-value database.
> More information: <https://redis.io>.

#### Start Redis server, using the default port (6379), and write logs to stdout:
```shell
redis-server
```
#### Start Redis server, using the default port, as a background process:
```shell
redis-server --daemonize yes
```
#### Start Redis server, using the specified port, as a background process:
```shell
redis-server --port {{port}} --daemonize yes
```
#### Start Redis server with a custom configuration file:
```shell
redis-server {{path/to/redis.conf}}
```
#### Start Redis server with verbose logging:
```shell
redis-server --loglevel {{warning|notice|verbose|debug}}
```
{% endraw %}