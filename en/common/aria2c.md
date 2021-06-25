---
layout: default
title: "aria2c"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aria2c">
  <a href="/en/common/aria2c.html">aria2c</a> <a href="#aria2c"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Fast download utility.
> Supports HTTP(S), FTP, SFTP, BitTorrent, and Metalink.
> More information: <https://aria2.github.io>.

#### Download a URI to a file:
```shell
aria2c {{url}}
```
#### Download the file pointed to by the specified URI with the specified output name:
```shell
aria2c --out={{filename}} {{url}}
```
#### Download multiple files in parallel:
```shell
aria2c --force-sequential {{url_1}} {{url_2}}
```
#### Download from multiple sources each URI pointing to the same file:
```shell
aria2c {{url_1}} {{url_2}}
```
#### Download the URIs listed in a file with limited parallel downloads:
```shell
aria2c --input-file={{filename}} --max-concurrent-downloads={{number_of_downloads}}
```
#### Download with multiple connections:
```shell
aria2c --split={{number_of_connections}} {{url}}
```
#### FTP download with username and password:
```shell
aria2c --ftp-user={{username}} --ftp-passwd={{password}} {{url}}
```
#### Limit download speed in bytes/s:
```shell
aria2c --max-download-limit={{speed}} {{url}}
```
{% endraw %}