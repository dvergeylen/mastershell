---
layout: default
title: "gunicorn"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gunicorn">
  <a href="/zh/common/gunicorn.html">gunicorn</a> <a href="#gunicorn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Python 的 WSGI http 服务器.

#### 运行 python web 应用程序:
```shell
gunicorn {{导入路径：应用程序}}
```
#### 在 localhost 上监听 8080 端口:
```shell
gunicorn --bind {{localhost}}:{{8080}} {{导入路径：应用程序}}
```
#### 启用实时自动加载:
```shell
gunicorn --reload {{导入路径：应用程序}}
```
#### 使用 4 个工作进程处理请求:
```shell
gunicorn --workers {{4}} {{导入路径：应用程序}}
```
#### 使用 4 个工作线程处理请求:
```shell
gunicorn --threads {{4}} {{导入路径：应用程序}}
```
#### 通过 https 运行应用程序:
```shell
gunicorn --certfile {{cert.pem}} --keyfile {{key.pem}} {{导入路径：应用程序}}
```
{% endraw %}