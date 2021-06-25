---
layout: default
title: "collectd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="collectd">
  <a href="/en/linux/collectd.html">collectd</a> <a href="#collectd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> System statistics collection daemon.
> More information: <https://collectd.org/>.

#### Show usage help, including the program version:
```shell
collectd -h
```
#### Test the configuration file and then exit:
```shell
collectd -t
```
#### Test plugin data collection functionality and then exit:
```shell
collectd -T
```
#### Start collectd:
```shell
collectd
```
#### Specify a custom configuration file location:
```shell
collectd -C {{path/to/file}}
```
#### Specify a custom PID file location:
```shell
collectd -P {{path/to/file}}
```
#### Don't fork into the background:
```shell
collectd -f
```
{% endraw %}