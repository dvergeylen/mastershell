---
layout: default
title: "pkill"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pkill">
  <a href="/en/common/pkill.html">pkill</a> <a href="#pkill"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Signal process by name.
> Mostly used for stopping processes.
> More information: <https://www.man7.org/linux/man-pages/man1/pkill.1.html>.

#### Kill all processes which match:
```shell
pkill -9 "{{process_name}}"
```
#### Kill all processes which match their full command instead of just the process name:
```shell
pkill -9 --full "{{command_name}}"
```
#### Send SIGUSR1 signal to processes which match:
```shell
pkill -USR1 "{{process_name}}"
```
#### Kill the main `firefox` process to close the browser:
```shell
pkill --oldest "{{firefox}}"
```
{% endraw %}