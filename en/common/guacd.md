---
layout: default
title: "guacd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="guacd">
  <a href="/en/common/guacd.html">guacd</a> <a href="#guacd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apache Guacamole proxy daemon.
> Support loader for client plugins to interface between the Guacamole protocol and any arbitrary remote desktop protocol (e.g. RDP, VNC, Other).
> More information: <https://guacamole.apache.org/>.

#### Bind to a specific port on localhost:
```shell
guacd -b {{127.0.0.1}} -l {{4823}}
```
#### Start in debug mode, keeping the process in the foreground:
```shell
guacd -f -L {{debug}}
```
#### Start with TLS support:
```shell
guacd -C {{my-cert.crt}} -K {{my-key.pem}}
```
#### Write the PID to a file:
```shell
guacd -p {{path/to/file.pid}}
```
{% endraw %}