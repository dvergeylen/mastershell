---
layout: default
title: "live-server"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="live-server">
  <a href="/en/common/live-server.html">live-server</a> <a href="#live-server"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A simple development http server with live reload capability.
> More information: <https://www.npmjs.com/package/live-server>.

#### Serve an `index.html` file and reload on changes:
```shell
live-server
```
#### Specify a port (default is 8080) from which to serve a file:
```shell
live-server --port={{8081}}
```
#### Specify a given file to serve:
```shell
live-server --open={{about.html}}
```
#### Proxy all requests for ROUTE to URL:
```shell
live-server --proxy={{/}}:{{http:localhost:3000}}
```
{% endraw %}