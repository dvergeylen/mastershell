---
layout: default
title: "tcpkill"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tcpkill">
  <a href="/en/linux/tcpkill.html">tcpkill</a> <a href="#tcpkill"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kills specified in-progress TCP connections.

#### Kill in-progress connections at a specified interface, host and port:
```shell
tcpkill -i {{eth1}} host {{192.95.4.27}} and port {{2266}}
```
{% endraw %}