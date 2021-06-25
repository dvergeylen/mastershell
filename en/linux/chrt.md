---
layout: default
title: "chrt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chrt">
  <a href="/en/linux/chrt.html">chrt</a> <a href="#chrt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manipulate the real-time attributes of a process.
> More information: <https://man7.org/linux/man-pages/man1/chrt.1.html>.

#### Display attributes of a process:
```shell
chrt --pid {{PID}}
```
#### Display attributes of all threads of a process:
```shell
chrt --all-tasks --pid {{PID}}
```
#### Display the min/max priority values that can be used with `chrt`:
```shell
chrt --max
```
#### Set the scheduling policy for a process:
```shell
chrt --pid {{PID}} --{{deadline|idle|batch|rr|fifo|other}}
```
{% endraw %}