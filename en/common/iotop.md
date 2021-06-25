---
layout: default
title: "iotop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="iotop">
  <a href="/en/common/iotop.html">iotop</a> <a href="#iotop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display a table of current I/O usage by processes or threads.
> More information: <https://manned.org/iotop>.

#### Start top-like I/O monitor:
```shell
sudo iotop
```
#### Show only processes or threads actually doing I/O:
```shell
sudo iotop --only
```
#### Show I/O usage in non-interactive mode:
```shell
sudo iotop --batch
```
#### Show only I/O usage of processes (default is to show all threads):
```shell
sudo iotop --processes
```
#### Show I/O usage of given PID(s):
```shell
sudo iotop --pid={{PID}}
```
#### Show I/O usage of a given user:
```shell
sudo iotop --user={{user}}
```
#### Show accumulated I/O instead of bandwidth:
```shell
sudo iotop --accumulated
```
{% endraw %}