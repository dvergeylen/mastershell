---
layout: default
title: "top"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="top">
  <a href="/en/linux/top.html">top</a> <a href="#top"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display dynamic real-time information about running processes.

#### Start top:
```shell
top
```
#### Do not show any idle or zombie processes:
```shell
top -i
```
#### Show only processes owned by given user:
```shell
top -u {{username}}
```
#### Sort processes by a field:
```shell
top -o {{field_name}}
```
#### Show the individual threads of a given process:
```shell
top -Hp {{process_id}}
```
#### Show only the processes with the given PID(s), passed as a comma-separated list. (Normally you wouldn't know PIDs off hand. This example picks the PIDs from the process name):
```shell
top -p $(pgrep -d ',' {{process_name}})
```
#### Get help about interactive commands:
```shell
?
```
{% endraw %}