---
layout: default
title: "scutil"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="scutil">
  <a href="/en/osx/scutil.html">scutil</a> <a href="#scutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage system configuration parameters.
> Necessitates to be root when setting configuration.

#### Display DNS Configuration:
```shell
scutil --dns
```
#### Display proxy configuration:
```shell
scutil --proxy
```
#### Get computer name:
```shell
scutil --get ComputerName
```
#### Set computer name:
```shell
sudo scutil --set ComputerName {{computer_name}}
```
#### Get hostname:
```shell
scutil --get HostName
```
#### Set hostname:
```shell
scutil --set HostName {{hostname}}
```
{% endraw %}