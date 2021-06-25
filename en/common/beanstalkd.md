---
layout: default
title: "beanstalkd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="beanstalkd">
  <a href="/en/common/beanstalkd.html">beanstalkd</a> <a href="#beanstalkd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A simple and generic work-queue server.
> More information: <https://beanstalkd.github.io/>.

#### Start beanstalkd, listening on port 11300:
```shell
beanstalkd
```
#### Start beanstalkd listening on a custom port and address:
```shell
beanstalkd -l {{ip_address}} -p {{port_number}}
```
#### Persist work queues by saving them to disk:
```shell
beanstalkd -b {{path/to/persistence_directory}}
```
#### Sync to the persistence directory every 500 milliseconds:
```shell
beanstalkd -b {{path/to/persistence_directory}} -f {{500}}
```
{% endraw %}