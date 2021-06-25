---
layout: default
title: "enum4linux"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="enum4linux">
  <a href="/en/linux/enum4linux.html">enum4linux</a> <a href="#enum4linux"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for enumerating Windows and Samba information from remote systems.
> It attempts to offer similar functionality to enum.exe formerly available from www.bindview.com.

#### Try to enumerate using all methods:
```shell
enum4linux -a {{remote_host}}
```
#### Enumerate using given login credentials:
```shell
enum4liux -u {{user_name}} -p {{password}} {{remote_host}}
```
#### List usernames from a given host:
```shell
enum4liux -U {{remote_host}}
```
#### List shares:
```shell
enum4liux -S {{remote_host}}
```
#### Get OS information:
```shell
enum4liux -o {{remote_host}}
```
{% endraw %}