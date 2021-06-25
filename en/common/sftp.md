---
layout: default
title: "sftp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sftp">
  <a href="/en/common/sftp.html">sftp</a> <a href="#sftp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Secure File Transfer Program.
> Interactive program to copy files between hosts over SSH.
> For non-interactive file transfers, see `scp` or `rsync`.

#### Connect to a remote server and enter an interactive command mode:
```shell
sftp {{remote_user}}@{{remote_host}}
```
#### Connect using an alternate port:
```shell
sftp -P {{remote_port}} {{remote_user}}@{{remote_host}}
```
#### Transfer remote file to the local system:
```shell
get {{/path/remote_file}}
```
#### Transfer local file to the remote system:
```shell
put {{/path/local_file}}
```
#### Transfer remote directory to the local system recursively (works with `put` too):
```shell
get -R {{/path/remote_directory}}
```
#### Get list of files on local machine:
```shell
lls
```
#### Get list of files on remote machine:
```shell
ls
```
{% endraw %}