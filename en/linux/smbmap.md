---
layout: default
title: "smbmap"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="smbmap">
  <a href="/en/linux/smbmap.html">smbmap</a> <a href="#smbmap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> SMB enumeration tool.
> More information: <https://github.com/ShawnDEvans/smbmap>.

#### Display SMB shares and permissions on a host, prompting for user's password or NTLM hash:
```shell
smbmap -u {{username}} --prompt -H {{ip}}
```
#### Display SMB shares and permissions on a host, specifying the domain and passing the password NTLM hash:
```shell
smbmap -u {{username}} --prompt -d {{domain}} -H {{ip}}
```
#### Display SMB shares and list a single level of directories and files:
```shell
smbmap -u {{username}} --prompt -H {{ip}} -r
```
#### Display SMB shares and recursively list a defined number of levels of directories and files:
```shell
smbmap -u {{username}} --prompt -H {{ip}} -R --depth {{3}}
```
#### Display SMB shares and recursively list directories and files, downloading the files matching a regular expression:
```shell
smbmap -u {{username}} --prompt -H {{ip}} -R -A {{pattern}}
```
#### Display SMB shares and recursively list directories and files, searching for file content matching a regular expression:
```shell
smbmap -u {{username}} --prompt -H {{ip}} -R -F {{pattern}}
```
#### Execute a shell command on a remote system:
```shell
smbmap -u {{username}} --prompt -H {{ip}} -x {{command}}
```
#### Upload a file to a remote system:
```shell
smbmap -u {{username}} --prompt -H {{ip}} --upload {{source}} {{destination}}
```
{% endraw %}