---
layout: default
title: "speed-test"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="speed-test">
  <a href="/en/common/speed-test.html">speed-test</a> <a href="#speed-test"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Test your internet connection speed and ping using speedtest.net from the CLI.
> More information: <https://github.com/sindresorhus/speed-test>.

#### Test your internet connection and ping speed:
```shell
speed-test
```
#### Output the results as JSON:
```shell
speed-test --json
```
#### Output the results in megabytes per second (MBps):
```shell
speed-test --bytes
```
#### Output more detailed information:
```shell
speed-test --verbose
```
{% endraw %}