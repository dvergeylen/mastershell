---
layout: default
title: "http"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="http">
  <a href="/en/common/http.html">http</a> <a href="#http"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> HTTPie: HTTP client, aims to be easier to use than cURL.
> More information: <https://httpie.org>.

#### Download a URL to a file:
```shell
http --download {{example.org}}
```
#### Send form-encoded data:
```shell
http --form {{example.org}} {{name='bob'}} {{profile_picture@'bob.png'}}
```
#### Send JSON object:
```shell
http {{example.org}} {{name='bob'}}
```
#### Specify an HTTP method:
```shell
http {{HEAD}} {{example.org}}
```
#### Include an extra header:
```shell
http {{example.org}} {{X-MyHeader:123}}
```
#### Pass a user name and password for server authentication:
```shell
http --auth {{username:password}} {{example.org}}
```
#### Specify raw request body via stdin:
```shell
cat {{data.txt}} | http PUT {{example.org}}
```
{% endraw %}