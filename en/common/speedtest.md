---
layout: default
title: "speedtest"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="speedtest">
  <a href="/en/common/speedtest.html">speedtest</a> <a href="#speedtest"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Official command-line interface for testing internet bandwidth using https://speedtest.net.
> Note: some platforms link `speedtest` to `speedtest-cli`. If some of the examples in this page don't work, see `speedtest-cli`.
> More information: <https://www.speedtest.net/apps/cli>.

#### Run a speed test:
```shell
speedtest
```
#### Run a speed test and specify the unit of the output:
```shell
speedtest --unit={{auto-decimal-bits|auto-decimal-bytes|auto-binary-bits|auto-binary-bytes}}
```
#### Run a speed test and specify the output format:
```shell
speedtest --format={{human-readable|csv|tsv|json|jsonl|json-pretty}}
```
#### Run a speed test and specify the number of decimal points to use (0 to 8, defaults to 2):
```shell
speedtest --precision={{precision}}
```
#### Run a speed test and print it's progress (only available for output format `human-readable` and `json`):
```shell
speedtest --progress={{yes|no}}
```
#### List all `speedtest.net` servers, sorted by distance:
```shell
speedtest --servers
```
#### Run a speed test to a specific `speedtest.net` server:
```shell
speedtest --server-id={{server_id}}
```
{% endraw %}