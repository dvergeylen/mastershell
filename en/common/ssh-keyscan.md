---
layout: default
title: "ssh-keyscan"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ssh-keyscan">
  <a href="/en/common/ssh-keyscan.html">ssh-keyscan</a> <a href="#ssh-keyscan"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get the public ssh keys of remote hosts.

#### Retrieve all public ssh keys of a remote host:
```shell
ssh-keyscan {{host}}
```
#### Retrieve all public ssh keys of a remote host listening on a specific port:
```shell
ssh-keyscan -p {{port}} {{host}}
```
#### Retrieve certain types of public ssh keys of a remote host:
```shell
ssh-keyscan -t {{rsa,dsa,ecdsa,ed25519}} {{host}}
```
#### Manually update the ssh known_hosts file with the fingerprint of a given host:
```shell
ssh-keyscan -H {{host}} >> ~/.ssh/known_hosts
```
{% endraw %}