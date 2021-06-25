---
layout: default
title: "ngrok"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ngrok">
  <a href="/en/common/ngrok.html">ngrok</a> <a href="#ngrok"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reverse proxy that creates a secure tunnel from a public endpoint to a locally running web service.
> More information: <https://ngrok.com>.

#### Expose a local HTTP service on a given port:
```shell
ngrok http {{80}}
```
#### Expose a local HTTP service on a specific host:
```shell
ngrok http {{foo.dev}}:{{80}}
```
#### Expose a local HTTPS server:
```shell
ngrok http https://localhost
```
#### Expose TCP traffic on a given port:
```shell
ngrok tcp {{22}}
```
#### Expose TLS traffic for a specific host and port:
```shell
ngrok tls -hostname={{foo.com}} {{443}}
```
{% endraw %}