---
layout: default
title: "traefik"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="traefik">
  <a href="/en/common/traefik.html">traefik</a> <a href="#traefik"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A HTTP reverse proxy and load balancer.
> More information: <https://traefik.io>.

#### Start server with default config:
```shell
traefik
```
#### Start server with a custom config file:
```shell
traefik --c {{config_file}}.toml
```
#### Start server with cluster mode enabled:
```shell
traefik --cluster
```
#### Start server with web UI enabled:
```shell
traefik --web
```
{% endraw %}