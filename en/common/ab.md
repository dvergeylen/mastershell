---
layout: default
title: "ab"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ab">
  <a href="/en/common/ab.html">ab</a> <a href="#ab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apache HTTP server benchmarking tool.
> More information: <https://httpd.apache.org/docs/current/programs/ab.html>.

#### Execute 100 HTTP GET requests to a given URL:
```shell
ab -n {{100}} {{url}}
```
#### Execute 100 HTTP GET requests, in concurrent batches of 10, to a URL:
```shell
ab -n {{100}} -c {{10}} {{url}}
```
#### Execute 100 HTTP POST requests to a URL, using a JSON payload from a file:
```shell
ab -n {{100}} -T {{application/json}} -p {{path/to/file.json}} {{url}}
```
#### Use HTTP [K]eep Alive, i.e. perform multiple requests within one HTTP session:
```shell
ab -k {{url}}
```
#### Set the maximum number of seconds to spend for benchmarking:
```shell
ab -t {{60}} {{url}}
```
{% endraw %}