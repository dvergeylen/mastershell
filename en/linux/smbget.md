---
layout: default
title: "smbget"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="smbget">
  <a href="/en/linux/smbget.html">smbget</a> <a href="#smbget"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> `wget`-like utility for downloading files from SMB servers.
> More information: <https://www.samba.org/samba/docs/current/man-html/smbget.1.html>.

#### Download a file from a server:
```shell
smbget {{smb://server/share/file}}
```
#### Download a share or directory recursively:
```shell
smbget --recursive {{smb://server/share}}
```
#### Connect with a username and password:
```shell
smbget {{smb://server/share/file}} --user {{username%password}}
```
#### Require encrypted transfers:
```shell
smbget {{smb://server/share/file}} --encrypt
```
{% endraw %}