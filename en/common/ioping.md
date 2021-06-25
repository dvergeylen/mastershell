---
layout: default
title: "ioping"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ioping">
  <a href="/en/common/ioping.html">ioping</a> <a href="#ioping"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Monitor I/O latency in real time.
> More information: <https://github.com/koct9i/ioping>.

#### Show disk I/O latency using the default values and the current directory:
```shell
ioping .
```
#### Measure latency on /tmp using 10 requests of 1 megabyte each:
```shell
ioping -c 10 -s 1M /tmp
```
#### Measure disk seek rate on `/dev/sdX`:
```shell
ioping -R {{/dev/sdX}}
```
#### Measure disk sequential speed on `/dev/sdX`:
```shell
ioping -RL {{/dev/sdX}}
```
{% endraw %}