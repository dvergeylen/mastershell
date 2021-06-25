---
layout: default
title: "driverquery"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="driverquery">
  <a href="/en/windows/driverquery.html">driverquery</a> <a href="#driverquery"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information about installed device drivers.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/driverquery>.

#### Display a list of all installed device drivers:
```shell
driverquery
```
#### Display a list of drivers in the specified format:
```shell
driverquery /fo {{table|list|csv}}
```
#### Display a list of drivers with a column to indicate if they are signed:
```shell
driverquery /si
```
#### Exclude the header in the output list:
```shell
driverquery /nh
```
#### Display a list of drivers for a remote machine:
```shell
driverquery /s {{hostname}} /u {{username}} /p {{password}}
```
#### Display a list of drivers with verbose information:
```shell
driverquery /v
```
#### Display detailed usage information:
```shell
driverquery /?
```
{% endraw %}