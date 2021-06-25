---
layout: default
title: "smbclient"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="smbclient">
  <a href="/en/linux/smbclient.html">smbclient</a> <a href="#smbclient"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> FTP-like client to access SMB/CIFS resources on servers.

#### Connect to a share (user will be prompted for password; `exit` to quit the session):
```shell
smbclient {{//server/share}}
```
#### Connect with a different username:
```shell
smbclient {{//server/share}} --user {{username}}
```
#### Connect with a different workgroup:
```shell
smbclient {{//server/share}} --workgroup {{domain}} --user {{username}}
```
#### Connect with a username and password:
```shell
smbclient {{//server/share}} --user {{username%password}}
```
#### Download a file from the server:
```shell
smbclient {{//server/share}} --directory {{path/to/directory}} --command "get {{file.txt}}"
```
#### Upload a file to the server:
```shell
smbclient {{//server/share}} --directory {{path/to/directory}} --command "put {{file.txt}}"
```
{% endraw %}