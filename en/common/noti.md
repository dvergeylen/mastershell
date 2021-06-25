---
layout: default
title: "noti"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="noti">
  <a href="/en/common/noti.html">noti</a> <a href="#noti"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Monitor a process and trigger a banner notification.
> More information: <https://github.com/variadico/noti>.

#### Display a notification when tar finishes compressing files:
```shell
noti {{tar -cjf example.tar.bz2 example/}}
```
#### Display a notification even when you put it after the command to watch:
```shell
{{command_to_watch}}; noti
```
#### Monitor a process by PID and trigger a notification when the PID disappears:
```shell
noti -w {{process_id}}
```
{% endraw %}