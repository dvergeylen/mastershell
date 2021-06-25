---
layout: default
title: "nginx"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nginx">
  <a href="/en/common/nginx.html">nginx</a> <a href="#nginx"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Nginx web server.
> More information: <https://nginx.org/en/>.

#### Start server with the default config file:
```shell
nginx
```
#### Start server with a custom config file:
```shell
nginx -c {{config_file}}
```
#### Start server with a prefix for all relative paths in the config file:
```shell
nginx -c {{config_file}} -p {{prefix/for/relative/paths}}
```
#### Test the configuration without affecting the running server:
```shell
nginx -t
```
#### Reload the configuration by sending a signal with no downtime:
```shell
nginx -s reload
```
{% endraw %}