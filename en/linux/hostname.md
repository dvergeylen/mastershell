---
layout: default
title: "hostname"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hostname">
  <a href="/en/linux/hostname.html">hostname</a> <a href="#hostname"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show or set the system's host name.

#### Show current host name:
```shell
hostname
```
#### Show the network address of the host name:
```shell
hostname -i
```
#### Show all network addresses of the host:
```shell
hostname -I
```
#### Show the FQDN (Fully Qualified Domain Name):
```shell
hostname --fqdn
```
#### Set current host name:
```shell
hostname {{new_hostname}}
```
{% endraw %}