---
layout: default
title: "tcpflow"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tcpflow">
  <a href="/en/linux/tcpflow.html">tcpflow</a> <a href="#tcpflow"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Capture TCP traffic for debugging and analysis.

#### Show all data on the given interface and port:
```shell
tcpflow -c -i {{eth0}} port {{80}}
```
{% endraw %}