---
layout: default
title: "redis-cli"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="redis-cli">
  <a href="/en/common/redis-cli.html">redis-cli</a> <a href="#redis-cli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Opens a connection to a Redis server.
> More information: <https://redis.io/topics/rediscli>.

#### Connect to the local server:
```shell
redis-cli
```
#### Connect to a remote server on the default port (6379):
```shell
redis-cli -h {{host}}
```
#### Connect to a remote server specifying a port number:
```shell
redis-cli -h {{host}} -p {{port}}
```
#### Connect to a remote server specifying an URI:
```shell
redis-cli -u {{uri}}
```
#### Specify a password:
```shell
redis-cli -a {{password}}
```
#### Execute Redis command:
```shell
redis-cli {{redis_command}}
```
#### Connect to the local cluster:
```shell
redis-cli -c
```
{% endraw %}