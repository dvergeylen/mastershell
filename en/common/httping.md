---
layout: default
title: "httping"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="httping">
  <a href="/en/common/httping.html">httping</a> <a href="#httping"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Measure the latency and throughput of a web server.
> More information: <https://www.vanheusden.com/httping>.

#### Ping the specified URL:
```shell
httping -g {{url}}
```
#### Ping the web server on `host` and `port`:
```shell
httping -h {{host}} -p {{port}}
```
#### Ping the web server on `host` using a TLS connection:
```shell
httping -l -g https://{{host}}
```
#### Ping the web server on `host` using HTTP basic authentication:
```shell
httping -g http://{{host}} -U {{username}} -P {{password}}
```
{% endraw %}