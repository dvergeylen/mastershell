---
layout: default
title: "mitmproxy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mitmproxy">
  <a href="/en/common/mitmproxy.html">mitmproxy</a> <a href="#mitmproxy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An interactive man-in-the-middle HTTP proxy.
> More information: <https://mitmproxy.org>.

#### Start mitmproxy with default settings:
```shell
mitmproxy
```
#### Start mitmproxy bound to custom address and port:
```shell
mitmproxy -b {{ip_address}} -p {{port}}
```
{% endraw %}