---
layout: default
title: "ssh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ssh">
  <a href="/en/common/ssh.html">ssh</a> <a href="#ssh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Secure Shell is a protocol used to securely log onto remote systems.
> It can be used for logging or executing commands on a remote server.

#### Connect to a remote server:
```shell
ssh {{username}}@{{remote_host}}
```
#### Connect to a remote server with a specific identity (private key):
```shell
ssh -i {{path/to/key_file}} {{username}}@{{remote_host}}
```
#### Connect to a remote server using a specific port:
```shell
ssh {{username}}@{{remote_host}} -p {{2222}}
```
#### Run a command on a remote server:
```shell
ssh {{remote_host}} {{command -with -flags}}
```
#### SSH tunneling: Dynamic port forwarding (SOCKS proxy on localhost:1080):
```shell
ssh -D {{1080}} {{username}}@{{remote_host}}
```
#### SSH tunneling: Forward a specific port (localhost:9999 to example.org:80) along with disabling pseudo-[t]ty allocation and executio[n] of remote commands:
```shell
ssh -L {{9999}}:{{example.org}}:{{80}} -N -T {{username}}@{{remote_host}}
```
#### SSH jumping: Connect through a jumphost to a remote server (Multiple jump hops may be specified separated by comma characters):
```shell
ssh -J {{username}}@{{jump_host}} {{username}}@{{remote_host}}
```
#### Agent forwarding: Forward the authentication information to the remote machine (see `man ssh_config` for available options):
```shell
ssh -A {{username}}@{{remote_host}}
```
{% endraw %}