---
layout: default
title: "xcaddy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xcaddy">
  <a href="/en/common/xcaddy.html">xcaddy</a> <a href="#xcaddy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The custom build tool for the Caddy Web Server.
> More information: <https://github.com/caddyserver/xcaddy>.

#### Build Caddy server from source:
```shell
xcaddy build
```
#### Build Caddy server with a specific version (defaults to latest):
```shell
xcaddy build {{version}}
```
#### Build Caddy with a specific module:
```shell
xcaddy build --with {{module_name}}
```
#### Build Caddy and output to a specific file:
```shell
xcaddy build --output {{path/to/file}}
```
#### Build and run Caddy for a development plugin in the current directory:
```shell
xcaddy run
```
#### Build and run Caddy for a development plugin using a specific Caddy config:
```shell
xcaddy run --config {{path/to/file}}
```
{% endraw %}