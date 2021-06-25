---
layout: default
title: "mosquitto_sub"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mosquitto_sub">
  <a href="/en/common/mosquitto_sub.html">mosquitto_sub</a> <a href="#mosquitto_sub"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A simple MQTT version 3.1.1 client that will subscribe to topics and print the messages that it receives.
> More information: <https://mosquitto.org/man/mosquitto_sub-1.html>.

#### Subscribe to the topic `sensors/temperature` information with Quality of Service (`QoS`) set to 1. (The default hostname is `localhost` and port 1883):
```shell
mosquitto_sub -t {{sensors/temperature}} -q {{1}}
```
#### Subscribe to all broker status messages publishing on `iot.eclipse.org` port 1885 and print published messages verbosely:
```shell
mosquitto_sub -v -h "iot.eclipse.org" -p 1885 -t {{\$SYS/#}}
```
#### Subscribe to multiple topics matching a given pattern. (+ takes any metric name):
```shell
mosquitto_sub -t {{sensors/machines/+/temperature/+}}
```
{% endraw %}