---
layout: default
title: "mosquitto"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mosquitto">
  <a href="/en/common/mosquitto.html">mosquitto</a> <a href="#mosquitto"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An MQTT broker.
> More information: <https://mosquitto.org/>.

#### Start mosquitto:
```shell
mosquitto
```
#### Specify a configuration file to use:
```shell
mosquitto --config-file {{path/to/file.conf}}
```
#### Listen on a specific port:
```shell
mosquitto --port {{8883}}
```
#### Daemonize by forking into the background:
```shell
mosquitto --daemon
```
{% endraw %}