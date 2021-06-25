---
layout: default
title: "openconnect"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="openconnect">
  <a href="/en/common/openconnect.html">openconnect</a> <a href="#openconnect"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A VPN client, for Cisco AnyConnect VPNs and others.
> More information: <https://www.infradead.org/openconnect/manual.html>.

#### Connect to a server:
```shell
openconnect {{vpn.example.org}}
```
#### Connect to a server, forking into the background:
```shell
openconnect --background {{vpn.example.org}}
```
#### Terminate the connection that is running in the background:
```shell
killall -SIGINT openconnect
```
#### Connect to a server, reading options from a config file:
```shell
openconnect --config={{path/to/file}} {{vpn.example.org}}
```
#### Connect to a server and authenticate with a specific SSL client certificate:
```shell
openconnect --certificate={{path/to/file}} {{vpn.example.org}}
```
{% endraw %}