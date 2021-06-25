---
layout: default
title: "journalctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="journalctl">
  <a href="/en/linux/journalctl.html">journalctl</a> <a href="#journalctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Query the systemd journal.

#### Show all messages from this [b]oot:
```shell
journalctl -b
```
#### Show all messages from last [b]oot:
```shell
journalctl -b -1
```
#### Show all messages with priority level 3 (errors) from this [b]oot:
```shell
journalctl -b --priority={{3}}
```
#### [f]ollow new messages (like `tail -f` for traditional syslog):
```shell
journalctl -f
```
#### Show all messages by a specific [u]nit:
```shell
journalctl -u {{unit}}
```
#### Filter messages within a time range (either timestamp or placeholders like "yesterday"):
```shell
journalctl --since {{now|today|yesterday|tomorrow}} --until {{YYYY-MM-DD HH:MM:SS}}
```
#### Show all messages by a specific process:
```shell
journalctl _PID={{pid}}
```
#### Show all messages by a specific executable:
```shell
journalctl {{path/to/executable}}
```
{% endraw %}