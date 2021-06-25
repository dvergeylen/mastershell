---
layout: default
title: "getmac"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="getmac">
  <a href="/en/windows/getmac.html">getmac</a> <a href="#getmac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the MAC addresses of a system.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/getmac>.

#### Display the MAC addresses for the current system:
```shell
getmac
```
#### Display the details in a specific format:
```shell
getmac /fo {{table|list|csv}}
```
#### Exclude the header in the output list:
```shell
getmac /nh
```
#### Display the MAC addresses for a remote machine:
```shell
getmac /s {{hostname}} /u {{username}} /p {{password}}
```
#### Display the MAC addresses with verbose information:
```shell
getmac /v
```
#### Display detailed usage information:
```shell
getmac /?
```
{% endraw %}