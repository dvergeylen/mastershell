---
layout: default
title: "caddy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="caddy">
  <a href="/en/common/caddy.html">caddy</a> <a href="#caddy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A powerful, enterprise-ready, open source web server with automatic HTTPS, written in Go.
> More information: <https://caddyserver.com>.

#### Start Caddy in the foreground:
```shell
caddy run
```
#### Start Caddy with the specified Caddyfile:
```shell
caddy run --config {{path/to/Caddyfile}}
```
#### Start Caddy in the background:
```shell
caddy start
```
#### Stop a background Caddy process:
```shell
caddy stop
```
#### Run a simple file server on the specified port with a browsable interface:
```shell
caddy file-server --listen :{{8000}} --browse
```
#### Run a reverse proxy server:
```shell
caddy reverse-proxy --from :{{80}} --to localhost:{{8000}}
```
{% endraw %}