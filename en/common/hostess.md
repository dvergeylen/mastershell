---
layout: default
title: "hostess"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hostess">
  <a href="/en/common/hostess.html">hostess</a> <a href="#hostess"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An idempotent command-line utility for managing the `/etc/hosts` file.
> More information: <https://github.com/cbednarski/hostess>.

#### List domains, target ips and on/off status:
```shell
hostess list
```
#### Add a domain pointing to your machine to your hosts file:
```shell
hostess add {{local.example.com}} {{127.0.0.1}}
```
#### Remove a domain from your hosts file:
```shell
hostess del {{local.example.com}}
```
#### Disable a domain (but don't remove it completely):
```shell
hostess off {{local.example.com}}
```
{% endraw %}