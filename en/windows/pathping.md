---
layout: default
title: "pathping"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pathping">
  <a href="/en/windows/pathping.html">pathping</a> <a href="#pathping"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A trace route tool combining features of `ping` and `tracert`.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/pathping>.

#### Ping and trace the route to a host:
```shell
pathping {{hostname}}
```
#### Do not perform reverse lookup of ip-address to hostname:
```shell
pathping {{hostname}} -n
```
#### Specify the maximum number of hops to search for the target (the default is 30):
```shell
pathping {{hostname}} -h {{max_hops}}
```
#### Specify the milliseconds to wait between pings (the default is 240):
```shell
pathping {{hostname}} -p {{time}}
```
#### Specify the number of queries per hop (the default is 100):
```shell
pathping {{hostname}} -q {{queries}}
```
#### Force IPV4 usage:
```shell
pathping {{hostname}} -4
```
#### Force IPV6 usage:
```shell
pathping {{hostname}} -6
```
#### Display detailed usage information:
```shell
pathping /?
```
{% endraw %}