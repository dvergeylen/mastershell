---
layout: default
title: "xh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xh">
  <a href="/en/common/xh.html">xh</a> <a href="#xh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Friendly and fast tool for sending HTTP requests.
> More information: <https://github.com/ducaale/xh>.

#### Send a GET request:
```shell
xh {{httpbin.org/get}}
```
#### Send a POST request with a JSON body (key-value pairs are added to a top-level JSON object - e.g. `{"name": "john", "age": 25}`):
```shell
xh post {{httpbin.org/post}} {{name=john}} {{age:=25}}
```
#### Send a GET request with query parameters (e.g. `first_param=5&second_param=true`):
```shell
xh get {{httpbin.org/get}} {{first_param==5}} {{second_param==true}}
```
#### Send a GET request with a custom header:
```shell
xh get {{httpbin.org/get}} {{header-name:header-value}}
```
#### Make a GET request and save the response body to a file:
```shell
xh --download {{httpbin.org/json}} --output {{path/to/file}}
```
{% endraw %}