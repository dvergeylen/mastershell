---
layout: default
title: "htpdate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="htpdate">
  <a href="/en/linux/htpdate.html">htpdate</a> <a href="#htpdate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Synchronize local date and time via HTTP headers from web servers.
> More information: <http://www.vervest.org/htp/>.

#### Synchronize date and time:
```shell
sudo htpdate {{host}}
```
#### Perform simulation of synchronization, without any action:
```shell
htpdate -q {{host}}
```
#### Compensate the systematisch clock drift:
```shell
sudo htpdate -x {{host}}
```
#### Set time immediate after the synchronization:
```shell
sudo htpdate -s {{host}}
```
{% endraw %}