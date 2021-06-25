---
layout: default
title: "timeout"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="timeout">
  <a href="/en/common/timeout.html">timeout</a> <a href="#timeout"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run a command with a time limit.
> More information: <https://www.gnu.org/software/coreutils/timeout>.

#### Run `sleep 10` and terminate it, if it runs for more than 3 seconds:
```shell
timeout {{3s}} {{sleep 10}}
```
#### Specify the signal to be sent to the command after the time limit expires. (By default, TERM is sent):
```shell
timeout --signal {{INT}} {{5s}} {{sleep 10}}
```
{% endraw %}