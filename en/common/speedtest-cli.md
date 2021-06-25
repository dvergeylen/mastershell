---
layout: default
title: "speedtest-cli"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="speedtest-cli">
  <a href="/en/common/speedtest-cli.html">speedtest-cli</a> <a href="#speedtest-cli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Unofficial command-line interface for testing internet bandwidth using https://speedtest.net.
> See also `speedtest` for the official CLI.
> More information: <https://github.com/sivel/speedtest-cli>.

#### Run a speed test:
```shell
speedtest-cli
```
#### Run a speed test and display values in bytes, instead of bits:
```shell
speedtest-cli --bytes
```
#### Run a speed test using `HTTPS`, instead of `HTTP`:
```shell
speedtest-cli --secure
```
#### Run a speed test without performing download tests:
```shell
speedtest-cli --no-download
```
#### Run a speed test and generate an image of the results:
```shell
speedtest-cli --share
```
#### List all `speedtest.net` servers, sorted by distance:
```shell
speedtest-cli --list
```
#### Run a speed test to a specific speedtest.net server:
```shell
speedtest-cli --server {{server_id}}
```
#### Run a speed test and display the results as JSON (suppresses progress information):
```shell
speedtest-cli --json
```
{% endraw %}