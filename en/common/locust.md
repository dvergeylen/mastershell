---
layout: default
title: "locust"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="locust">
  <a href="/en/common/locust.html">locust</a> <a href="#locust"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Load-testing tool to determine number of concurrent users a system can handle.
> More information: <https://locust.io>.

#### Load-test "example.com" with web interface using locustfile.py:
```shell
locust --host={{http://example.com}}
```
#### Use a different test file:
```shell
locust --locustfile={{test_file.py}} --host={{http://example.com}}
```
#### Run test without web interface, spawning 1 user a second until there are 100 users:
```shell
locust --no-web --clients={{100}} --hatch-rate={{1}} --host={{http://example.com}}
```
#### Start locust in master mode:
```shell
locust --master --host={{http://example.com}}
```
#### Connect locust slave to master:
```shell
locust --slave --host={{http://example.com}}
```
#### Connect locust slave to master on a different machine:
```shell
locust --slave --master-host={{master_hostname}} --host={{http://example.com}}
```
{% endraw %}