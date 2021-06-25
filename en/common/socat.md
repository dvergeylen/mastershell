---
layout: default
title: "socat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="socat">
  <a href="/en/common/socat.html">socat</a> <a href="#socat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Multipurpose relay (SOcket CAT).

#### Listen to a port, wait for an incoming connection and transfer data to STDIO:
```shell
socat - TCP-LISTEN:8080,fork
```
#### Create a connection to a host and port, transfer data in STDIO to connected host:
```shell
socat - TCP4:www.example.com:80
```
#### Forward incoming data of a local port to another host and port:
```shell
socat TCP-LISTEN:80,fork TCP4:www.example.com:80
```
{% endraw %}