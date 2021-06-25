---
layout: default
title: "httpry"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="httpry">
  <a href="/en/common/httpry.html">httpry</a> <a href="#httpry"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A lightweight packet sniffer for displaying and logging HTTP traffic.
> It can be run in real-time displaying the traffic as it is parsed, or as a daemon process that logs to an output file.
> More information: <http://dumpsterventures.com/jason/httpry/>.

#### Save output to a file:
```shell
httpry -o {{path/to/file.log}}
```
#### Listen on a specific interface and save output to a binary pcap format file:
```shell
httpry {{eth0}} -b {{path/to/file.pcap}}
```
#### Filter output by a comma-separated list of HTTP verbs:
```shell
httpry -m {{get|post|put|head|options|delete|trace|connect|patch}}
```
#### Read from an input capture file and filter by IP:
```shell
httpry -r {{path/to/file.log}} '{{host 192.168.5.25}}'
```
#### Run as daemon process:
```shell
httpry -d -o {{path/to/file.log}}
```
{% endraw %}