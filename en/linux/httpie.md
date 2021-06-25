---
layout: default
title: "httpie"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="httpie">
  <a href="/en/linux/httpie.html">httpie</a> <a href="#httpie"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A user friendly command-line HTTP tool.

#### Send a GET request (default method with no request data):
```shell
http {{https://example.com}}
```
#### Send a POST request (default method with request data):
```shell
http {{https://example.com}} {{hello=World}}
```
#### Send a POST request with redirected input:
```shell
http {{https://example.com}} < {{file.json}}
```
#### Send a PUT request with a given json body:
```shell
http PUT {{https://example.com/todos/7}} {{hello=world}}
```
#### Send a DELETE request with a given request header:
```shell
http DELETE {{https://example.com/todos/7}} {{API-Key:foo}}
```
#### Show the whole HTTP exchange (both request and response):
```shell
http -v {{https://example.com}}
```
#### Download a file:
```shell
http --download {{https://example.com}}
```
{% endraw %}