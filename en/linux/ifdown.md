---
layout: default
title: "ifdown"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ifdown">
  <a href="/en/linux/ifdown.html">ifdown</a> <a href="#ifdown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Disable network interfaces.
> More information: <https://manned.org/ifdown>.

#### Disable interface eth0:
```shell
ifdown {{eth0}}
```
#### Disable all interfaces which are enabled:
```shell
ifdown -a
```
{% endraw %}