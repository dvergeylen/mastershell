---
layout: default
title: "ftp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ftp">
  <a href="/en/common/ftp.html">ftp</a> <a href="#ftp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tools to interact with a server via File Transfer Protocol.

#### Connect to an FTP server:
```shell
ftp {{ftp.example.com}}
```
#### Switch to binary transfer mode (graphics, compressed files, etc):
```shell
binary
```
#### Transfer multiple files without prompting for confirmation on every file:
```shell
prompt off
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
#### Rename a file on the remote server:
```shell
rename {{original_filename}} {{new_filename}}
```
{% endraw %}