---
layout: default
title: "rpcinfo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rpcinfo">
  <a href="/en/windows/rpcinfo.html">rpcinfo</a> <a href="#rpcinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List programs via RPC on remote computers.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/rpcinfo>.

#### List all programs registered on the local computer:
```shell
rpcinfo
```
#### List all programs registered on a remote computer:
```shell
rpcinfo /p {{computer_name}}
```
#### Call a specific program on a remote computer using TCP:
```shell
rpcinfo /t {{computer_name}} {{program_name}}
```
#### Call a specific program on a remote computer using UDP:
```shell
rpcinfo /u {{computer_name}} {{program_name}}
```
{% endraw %}