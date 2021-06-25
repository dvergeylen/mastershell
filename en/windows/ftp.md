---
layout: default
title: "ftp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ftp">
  <a href="/en/windows/ftp.html">ftp</a> <a href="#ftp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interactively transfer files between a local and remote FTP server.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/ftp>.

#### Connect to a remote FTP server interactively:
```shell
ftp {{host}}
```
#### Log in as an anonymous user:
```shell
ftp -A {{host}}
```
#### Disable automatic login upon initial connection:
```shell
ftp -n {{host}}
```
#### Run a file containing a list of FTP commands:
```shell
ftp -s:{{path/to/file}} {{host}}
```
#### Download multiple files (glob expression):
```shell
mget {{*.png}}
```
#### Upload multiple files (glob expression):
```shell
mput {{*.zip}}
```
#### Delete multiple files on the remote server:
```shell
mdelete {{*.txt}}
```
#### Display detailed help:
```shell
ftp --help
```
{% endraw %}