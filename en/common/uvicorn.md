---
layout: default
title: "uvicorn"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="uvicorn">
  <a href="/en/common/uvicorn.html">uvicorn</a> <a href="#uvicorn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Python ASGI HTTP Server, for asynchronous projects.
> More information: <https://www.uvicorn.org/>.

#### Run Python web app:
```shell
uvicorn {{import.path:app_object}}
```
#### Listen on port 8080 on localhost:
```shell
uvicorn --host {{localhost}} --port {{8080}} {{import.path:app_object}}
```
#### Turn on live reload:
```shell
uvicorn --reload {{import.path:app_object}}
```
#### Use 4 worker processes for handling requests:
```shell
uvicorn --workers {{4}} {{import.path:app_object}}
```
#### Run app over HTTPS:
```shell
uvicorn --ssl-certfile {{cert.pem}} --ssl-keyfile {{key.pem}} {{import.path:app_object}}
```
{% endraw %}