---
layout: default
title: "openfortivpn"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="openfortivpn">
  <a href="/en/linux/openfortivpn.html">openfortivpn</a> <a href="#openfortivpn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A VPN client, for Fortinet's proprietary PPP+SSL VPN solution.
> More information: <https://github.com/adrienverge/openfortivpn>.

#### Connect to a VPN with a username and password:
```shell
openfortivpn --username={{username}} --password={{password}}
```
#### Connect to a VPN using a specific configuration file (defaults to `/etc/openfortivpn/config`):
```shell
sudo openfortivpn --config={{path/to/config}}
```
#### Connect to a VPN by specifying the host and port:
```shell
openfortivpn {{host}}:{{port}}
```
#### Trust a given gateway by passing in its certificate's sha256 sum:
```shell
openfortivpn --trusted-cert={{sha256_sum}}
```
{% endraw %}