---
layout: default
title: "mosh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mosh">
  <a href="/en/common/mosh.html">mosh</a> <a href="#mosh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mobile Shell (`mosh`) is a robust and responsive replacement for SSH.
> `mosh` persists connections to remote servers while roaming between networks.
> More information: <https://mosh.org>.

#### Connect to a remote server:
```shell
mosh {{username}}@{{remote_host}}
```
#### Connect to a remote server with a specific identity (private key):
```shell
mosh --ssh="ssh -i {{path/to/key_file}}" {{username}}@{{remote_host}}
```
#### Connect to a remote server using a specific port:
```shell
mosh --ssh="ssh -p {{2222}}" {{username}}@{{remote_host}}
```
#### Run a command on a remote server:
```shell
mosh {{remote_host}} -- {{command -with -flags}}
```
#### Select Mosh UDP port (useful when `{{remote_host}}` is behind a NAT):
```shell
mosh -p {{124}} {{username}}@{{remote_host}}
```
#### Usage when `mosh-server` binary is outside standard path:
```shell
mosh --server={{path/to/bin/}}mosh-server {{remote_host}}
```
{% endraw %}