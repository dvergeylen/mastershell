---
layout: default
title: "nc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nc">
  <a href="/en/common/nc.html">nc</a> <a href="#nc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Netcat is a versatile utility for working with TCP or UDP data.
> More information: <https://nmap.org/ncat>.

#### Listen on a specified port and print any data received:
```shell
nc -l {{port}}
```
#### Connect to a certain port:
```shell
nc {{ip_address}} {{port}}
```
#### Set a timeout:
```shell
nc -w {{timeout_in_seconds}} {{ipaddress}} {{port}}
```
#### Keep the server up after the client detaches:
```shell
nc -k -l {{port}}
```
#### Keep the client up even after EOF:
```shell
nc -q {{timeout}} {{ip_address}}
```
#### Scan the open ports of a specified host:
```shell
nc -v -z {{ip_address}} {{port}}
```
#### Act as proxy and forward data from a local TCP port to the given remote host:
```shell
nc -l {{local_port}} | nc {{hostname}} {{remote_port}}
```
{% endraw %}