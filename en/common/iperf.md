---
layout: default
title: "iperf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="iperf">
  <a href="/en/common/iperf.html">iperf</a> <a href="#iperf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Measure network bandwidth between computers.
> More information: <https://iperf.fr>.

#### Run on server:
```shell
iperf -s
```
#### Run on server using UDP mode and set server port to listen on 5001:
```shell
iperf -u -s -p {{5001}}
```
#### Run on client:
```shell
iperf -c {{server_address}}
```
#### Run on client every 2 seconds:
```shell
iperf -c {{server_address}} -i {{2}}
```
#### Run on client with 5 parallel threads:
```shell
iperf -c {{server_address}} -P {{5}}
```
#### Run on client using UDP mode:
```shell
iperf -u -c {{server_address}} -p {{5001}}
```
{% endraw %}