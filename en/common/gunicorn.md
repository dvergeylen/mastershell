---
layout: default
title: "gunicorn"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gunicorn">
  <a href="/en/common/gunicorn.html">gunicorn</a> <a href="#gunicorn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Python WSGI HTTP Server.
> More information: <https://gunicorn.org/>.

#### Run Python web app:
```shell
gunicorn {{import.path:app_object}}
```
#### Listen on port 8080 on localhost:
```shell
gunicorn --bind {{localhost}}:{{8080}} {{import.path:app_object}}
```
#### Turn on live reload:
```shell
gunicorn --reload {{import.path:app_object}}
```
#### Use 4 worker processes for handling requests:
```shell
gunicorn --workers {{4}} {{import.path:app_object}}
```
#### Use 4 worker threads for handling requests:
```shell
gunicorn --threads {{4}} {{import.path:app_object}}
```
#### Run app over HTTPS:
```shell
gunicorn --certfile {{cert.pem}} --keyfile {{key.pem}} {{import.path:app_object}}
```
{% endraw %}