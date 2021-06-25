---
layout: default
title: "darkhttpd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="darkhttpd">
  <a href="/en/common/darkhttpd.html">darkhttpd</a> <a href="#darkhttpd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Darkhttpd web server.
> More information: <https://unix4lyfe.org/darkhttpd>.

#### Start server serving the specified document root:
```shell
darkhttpd {{path/to/docroot}}
```
#### Start server on specified port (port 8080 by default if running as non-root user):
```shell
darkhttpd {{path/to/docroot}} --port {{port}}
```
#### Listen only on specified IP address (by default, the server listens on all interfaces):
```shell
darkhttpd {{path/to/docroot}} --addr {{ip_address}}
```
{% endraw %}