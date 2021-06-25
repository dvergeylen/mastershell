---
layout: default
title: "rpcinfo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rpcinfo">
  <a href="/en/linux/rpcinfo.html">rpcinfo</a> <a href="#rpcinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Makes an RPC call to an RPC server and reports what it finds.

#### Show full table of all RPC services registered on localhost:
```shell
rpcinfo
```
#### Show concise table of all RPC services registered on localhost:
```shell
rpcinfo -s {{localhost}}
```
#### Display table of statistics of rpcbind operations on localhost:
```shell
rpcinfo -m
```
#### Display list of entries of given service name (mountd) and version number (2) on a remote nfs share:
```shell
rpcinfo -l {{remote_nfs_server_ip}} {{mountd}} {{2}}
```
#### Delete the registration for version 1 of the mountd service for all transports:
```shell
rpcinfo -d {{mountd}} {{1}}
```
{% endraw %}