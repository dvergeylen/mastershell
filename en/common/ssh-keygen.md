---
layout: default
title: "ssh-keygen"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ssh-keygen">
  <a href="/en/common/ssh-keygen.html">ssh-keygen</a> <a href="#ssh-keygen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate ssh keys used for authentication, password-less logins, and other things.

#### Generate a key interactively:
```shell
ssh-keygen
```
#### Specify file in which to save the key:
```shell
ssh-keygen -f ~/.ssh/{{filename}}
```
#### Generate an ed25519 key with 100 key derivation function rounds:
```shell
ssh-keygen -t ed25519 -a 100
```
#### Generate an RSA 4096 bit key with email as a comment:
```shell
ssh-keygen -t rsa -b 4096 -C "{{email}}"
```
#### Retrieve the key fingerprint from a host (useful for confirming the authenticity of the host when first connecting to it via SSH):
```shell
ssh-keygen -l -F {{remote_host}}
```
#### Remove the keys of a host from the known_hosts file (useful when a known host has a new key):
```shell
ssh-keygen -R {{remote_host}}
```
#### Retrieve the fingerprint of a key in MD5 Hex:
```shell
ssh-keygen -l -E md5 -f ~/.ssh/{{filename}}
```
#### Change the password of a key:
```shell
ssh-keygen -p -f ~/.ssh/{{filename}}
```
{% endraw %}