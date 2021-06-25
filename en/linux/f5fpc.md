---
layout: default
title: "f5fpc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="f5fpc">
  <a href="/en/linux/f5fpc.html">f5fpc</a> <a href="#f5fpc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A proprietry commercial SSL VPN client by BIG-IP Edge.

#### Open a new VPN connection:
```shell
sudo f5fpc --start
```
#### Open a new VPN connection to a specific host:
```shell
sudo f5fpc --start --host {{host.example.com}}
```
#### Specify a username (user will be prompted for a password):
```shell
sudo f5fpc --start --host {{host.example.com}} --username {{user}}
```
#### Show the current VPN status:
```shell
sudo f5fpc --info
```
#### Shutdown the VPN connection:
```shell
sudo f5fpc --stop
```
{% endraw %}