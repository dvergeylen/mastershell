---
layout: default
title: "waitress-serve"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="waitress-serve">
  <a href="/en/common/waitress-serve.html">waitress-serve</a> <a href="#waitress-serve"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pure Python WSGI HTTP Server.

#### Run a Python web app:
```shell
waitress-serve {{import.path:wsgi_func}}
```
#### Listen on port 8080 on localhost:
```shell
waitress-serve --listen={{localhost}}:{{8080}} {{import.path:wsgi_func}}
```
#### Start waitress on a Unix socket:
```shell
waitress-serve --unix-socket={{path/to/socket}} {{import.path:wsgi_func}}
```
#### Use 4 threads to process requests:
```shell
waitress-serve --threads={{4}} {{import.path:wsgifunc}}
```
#### Call a factory method that returns a WSGI object:
```shell
waitress-serve --call {{import.path.wsgi_factory}}
```
#### Set the URL scheme to https:
```shell
waitress-serve --url-scheme={{https}} {{import.path:wsgi_func}}
```
{% endraw %}