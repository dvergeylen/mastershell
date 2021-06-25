---
layout: default
title: "logger"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="logger">
  <a href="/en/linux/logger.html">logger</a> <a href="#logger"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Add messages to syslog (/var/log/syslog).

#### Log a message to syslog:
```shell
logger {{message}}
```
#### Take input from stdin and log to syslog:
```shell
echo {{log_entry}} | logger
```
#### Send the output to a remote syslog server running at a given port. Default port is 514:
```shell
echo {{log_entry}} | logger --server {{hostname}} --port {{port}}
```
#### Use a specific tag for every line logged. Default is the name of logged in user:
```shell
echo {{log_entry}} | logger --tag {{tag}}
```
#### Log messages with a given priority. Default is `user.notice`. See `man logger` for all priority options:
```shell
echo {{log_entry}} | logger --priority {{user.warning}}
```
{% endraw %}