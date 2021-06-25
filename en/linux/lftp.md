---
layout: default
title: "lftp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lftp">
  <a href="/en/linux/lftp.html">lftp</a> <a href="#lftp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sophisticated file transfer program.
> More information: <https://lftp.yar.ru/lftp-man.html>.

#### Connect to an FTP server:
```shell
lftp {{ftp.example.com}}
```
#### Download multiple files (glob expression):
```shell
mget {{path/to/*.png}}
```
#### Upload multiple files (glob expression):
```shell
mput {{path/to/*.zip}}
```
#### Delete multiple files on the remote server:
```shell
mrm {{path/to/*.txt}}
```
#### Rename a file on the remote server:
```shell
mv {{original_filename}} {{new_filename}}
```
#### Download or update an entire directory:
```shell
mirror {{path/to/remote_dir}} {{path/to/local_output_dir}}
```
#### Upload or update an entire directory:
```shell
mirror -R {{path/to/local_dir}} {{path/to/remote_output_dir}}
```
{% endraw %}