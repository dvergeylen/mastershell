---
layout: default
title: "iperf3"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="iperf3">
  <a href="/en/common/iperf3.html">iperf3</a> <a href="#iperf3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Traffic generator for testing network bandwidth.
> More information: <https://iperf.fr>.

#### Run iperf3 as a server:
```shell
iperf3 -s
```
#### Run an iperf3 server on a specific port:
```shell
iperf3 -s -p {{port}}
```
#### Start bandwidth test:
```shell
iperf3 -c {{server}}
```
#### Run iperf3 in multiple parallel streams:
```shell
iperf3 -c {{server}} -P {{streams}}
```
#### Reverse direction of the test. Server sends data to the client:
```shell
iperf3 -c {{server}} -R
```
{% endraw %}