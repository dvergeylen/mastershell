---
layout: default
title: "watch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="watch">
  <a href="/en/common/watch.html">watch</a> <a href="#watch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Execute a program periodically, showing output fullscreen.

#### Repeatedly run a command and show the result:
```shell
watch {{command}}
```
#### Re-run a command every 60 seconds:
```shell
watch -n {{60}} {{command}}
```
#### Monitor the contents of a directory, highlighting differences as they appear:
```shell
watch -d {{ls -l}}
```
{% endraw %}