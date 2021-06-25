---
layout: default
title: "watch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="watch">
  <a href="/en/linux/watch.html">watch</a> <a href="#watch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Execute a command repeatedly, and monitor the output in full-screen mode.

#### Monitor files in the current directory:
```shell
watch {{ls}}
```
#### Monitor disk space and highlight the changes:
```shell
watch -d {{df}}
```
#### Monitor "node" processes, refreshing every 3 seconds:
```shell
watch -n {{3}} "{{ps aux | grep node}}"
```
{% endraw %}