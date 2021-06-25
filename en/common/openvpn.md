---
layout: default
title: "openvpn"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="openvpn">
  <a href="/en/common/openvpn.html">openvpn</a> <a href="#openvpn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> OpenVPN client and daemon binary.
> More information: <https://openvpn.net/>.

#### Connect to server using a config file:
```shell
sudo openvpn {{path/to/client.conf}}
```
#### Try to set up an insecure peer-to-peer tunnel on bob.example.com host:
```shell
sudo openvpn --remote {{alice.example.com}} --dev {{tun1}} --ifconfig {{10.4.0.1}} {{10.4.0.2}}
```
#### Connect to the awaiting bob.example.com host without encryption:
```shell
sudo openvpn --remote {{bob.example.com}} --dev {{tun1}} --ifconfig {{10.4.0.2}} {{10.4.0.1}}
```
#### Create a cryptographic key and save it to file:
```shell
openvpn --genkey --secret {{path/to/key}}
```
#### Try to set up a peer-to-peer tunnel on bob.example.com host with a static key:
```shell
sudo openvpn --remote {{alice.example.com}} --dev {{tun1}} --ifconfig {{10.4.0.1}} {{10.4.0.2}} --secret {{path/to/key}}
```
#### Connect to the awaiting bob.example.com host with the same static key as on bob.example.com:
```shell
sudo openvpn --remote {{bob.example.com}} --dev {{tun1}} --ifconfig {{10.4.0.2}} {{10.4.0.1}} --secret {{path/to/key}}
```
{% endraw %}