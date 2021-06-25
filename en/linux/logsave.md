---
layout: default
title: "logsave"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="logsave">
  <a href="/en/linux/logsave.html">logsave</a> <a href="#logsave"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Save the output of a command in a logfile.
> More information: <https://manned.org/logsave>.

#### Execute command with specified argument(s) and save its output to log file:
```shell
logsave {{path/to/logfile}} {{command}}
```
#### Take input from standard input and save it in a log file:
```shell
logsave {{logfile}} -
```
#### Append the output to a log file, instead of replacing its current contents:
```shell
logsave -a {{logfile}} {{command}}
```
#### Show verbose output:
```shell
logsave -v {{logfile}} {{command}}
```
{% endraw %}