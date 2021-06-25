---
layout: default
title: "http_load"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="http_load">
  <a href="/en/linux/http_load.html">http_load</a> <a href="#http_load"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A HTTP benchmarking tool.
> Runs multiple HTTP fetches in parallel to test the throughput of a web server.
> More information: <http://www.acme.com/software/http_load/>.

#### Emulate 20 requests based on a given URL list file per second for 60 seconds:
```shell
http_load -rate {{20}} -seconds {{60}} {{path/to/urls.txt}}
```
#### Emulate 5 concurrent requests based on a given URL list file for 60 seconds:
```shell
http_load -parallel {{5}} -seconds {{60}} {{path/to/urls.txt}}
```
#### Emulate 1000 requests at 20 requests per second, based on a given URL list file:
```shell
http_load -rate {{20}} -fetches {{1000}} {{path/to/urls.txt}}
```
#### Emulate 1000 requests at 5 concurrent requests at a time, based on a given URL list file:
```shell
http_load -parallel {{5}} -fetches {{1000}} {{path/to/urls.txt}}
```
{% endraw %}