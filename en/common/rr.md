---
layout: default
title: "rr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rr">
  <a href="/en/common/rr.html">rr</a> <a href="#rr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debugging tool designed to record and replay program execution.
> More information: <https://rr-project.org/>.

#### Record an application:
```shell
rr record {{path/to/binary --arg1 --arg2}}
```
#### Replay latest recorded execution:
```shell
rr replay
```
{% endraw %}