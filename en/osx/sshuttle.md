---
layout: default
title: "sshuttle"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sshuttle">
  <a href="/en/osx/sshuttle.html">sshuttle</a> <a href="#sshuttle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Transparent proxy server that tunnels traffic over an SSH connection.
> Doesn't require admin, or any special setup on the remote SSH server.
> More information: <https://github.com/sshuttle/sshuttle>.

#### Forward all IPv4 TCP traffic via a remote SSH server:
```shell
sshuttle --remote={{username}}@{{sshserver}} {{0.0.0.0/0}}
```
#### Forward all IPv4 TCP and DNS traffic:
```shell
sshuttle --dns --remote={{username}}@{{sshserver}} {{0.0.0.0/0}}
```
#### Use the tproxy method to forward all IPv4 and IPv6 traffic:
```shell
sudo sshuttle --method=tproxy --remote={{username}}@{{sshserver}} {{0.0.0.0/0}} {{::/0}} --exclude={{your_local_ip_address}} --exclude={{ssh_server_ip_address}}
```
{% endraw %}