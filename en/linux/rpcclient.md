---
layout: default
title: "rpcclient"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rpcclient">
  <a href="/en/linux/rpcclient.html">rpcclient</a> <a href="#rpcclient"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> MS-RPC client tool (part of the samba suite).
> More information: <https://www.samba.org/samba/docs/current/man-html/rpcclient.1.html>.

#### Connect to a remote host:
```shell
rpcclient --user {{domain}}\{{username}}%{{password}} {{ip}}
```
#### Connect to a remote host on a domain without a password:
```shell
rpcclient --user {{username}} --workgroup {{domain}} --no-pass {{ip}}
```
#### Connect to a remote host, passing the password hash:
```shell
rpcclient --user {{domain}}\{{username}} --pw-nt-hash {{ip}}
```
#### Execute shell commands on a remote host:
```shell
rpcclient --user {{domain}}\{{username}}%{{password}} --command {{semicolon_separated_commands}} {{ip}}
```
#### Display domain users:
```shell
rpcclient $> enumdomusers
```
#### Display privileges:
```shell
rpcclient $> enumprivs
```
#### Display information about a specific user:
```shell
rpcclient $> queryuser {{username|rid}}
```
#### Create a new user in the domain:
```shell
rpcclient $> createdomuser {{username}}
```
{% endraw %}