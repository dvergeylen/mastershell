---
layout: default
title: "lt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lt">
  <a href="/en/common/lt.html">lt</a> <a href="#lt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Localtunnel exposes your localhost to the world for easy testing and sharing.
> More information: <https://github.com/localtunnel/localtunnel>.

#### Start tunnel from a specific port:
```shell
lt --port {{8000}}
```
#### Specify the upstream server doing the forwarding:
```shell
lt --port {{8000}} --host {{host}}
```
#### Request a specific subdomain:
```shell
lt --port {{8000}} --subdomain {{subdomain}}
```
#### Print basic request info:
```shell
lt --port {{8000}} --print-requests
```
#### Open the tunnel URL in the default web browser:
```shell
lt --port {{8000}} --open
```
{% endraw %}