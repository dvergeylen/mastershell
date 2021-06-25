---
layout: default
title: "httpflow"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="httpflow">
  <a href="/en/common/httpflow.html">httpflow</a> <a href="#httpflow"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line utility to capture and dump HTTP streams.
> More information: <https://github.com/six-ddc/httpflow>.

#### Capture traffic on all interfaces:
```shell
httpflow -i {{any}}
```
#### Use a bpf-style capture to filter the results:
```shell
httpflow {{host httpbin.org or host baidu.com}}
```
#### Use a regular expression to filter requests by URLs:
```shell
httpflow -u '{{regular_expression}}'
```
#### Read packets from pcap format binary file:
```shell
httpflow -r {{out.cap}}
```
#### Write the output to a directory:
```shell
httpflow -w {{path/to/directory}}
```
{% endraw %}