---
layout: default
title: "tshark"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tshark">
  <a href="/en/linux/tshark.html">tshark</a> <a href="#tshark"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Packet analysis tool, CLI version of Wireshark.

#### Monitor everything on localhost:
```shell
tshark
```
#### Only capture packets matching a specific capture filter:
```shell
tshark -f '{{udp port 53}}'
```
#### Only show packets matching a specific output filter:
```shell
tshark -Y '{{http.request.method == "GET"}}'
```
#### Decode a TCP port using a specific protocol (e.g. HTTP):
```shell
tshark -d tcp.port=={{8888}},{{http}}
```
#### Specify the format of captured output:
```shell
tshark -T {{json|text|ps|…}}
```
#### Select specific fields to output:
```shell
tshark -T {{fields|ek|json|pdml}} -e {{http.request.method}} -e {{ip.src}}
```
#### Write captured packet to a file:
```shell
tshark -w {{path/to/file}}
```
#### Analyze packets from a file:
```shell
tshark -r {{filename}}.pcap
```
{% endraw %}