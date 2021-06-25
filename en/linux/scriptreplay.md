---
layout: default
title: "scriptreplay"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="scriptreplay">
  <a href="/en/linux/scriptreplay.html">scriptreplay</a> <a href="#scriptreplay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Replay a typescript created by the `script` command to the standard output.

#### Replay a typescript at the speed it was recorded:
```shell
scriptreplay {{path/to/timing_file}} {{path/to/typescript}}
```
#### Replay a typescript at double the original speed:
```shell
scriptreplay {{path/to/timingfile}} {{path/to/typescript}} 2
```
#### Replay a typescript at half the original speed:
```shell
scriptreplay {{path/to/timingfile}} {{path/to/typescript}} 0.5
```
{% endraw %}