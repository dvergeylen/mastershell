---
layout: default
title: "stress"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="stress">
  <a href="/en/linux/stress.html">stress</a> <a href="#stress"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to stress test CPU, memory, and IO on a Linux system.

#### Spawn 4 workers to stress test CPU:
```shell
stress -c {{4}}
```
#### Spawn 2 workers to stress test IO and timeout after 5 seconds:
```shell
stress -i {{2}} -t {{5}}
```
#### Spawn 2 workers to stress test memory (each worker allocates 256M bytes):
```shell
stress -m {{2}} --vm-bytes {{256M}}
```
#### Spawn 2 workers spinning on write()/unlink() (each worker writes 1G bytes):
```shell
stress -d {{2}} --hdd-bytes {{1GB}}
```
{% endraw %}