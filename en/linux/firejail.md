---
layout: default
title: "firejail"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="firejail">
  <a href="/en/linux/firejail.html">firejail</a> <a href="#firejail"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Securely sandboxes processes to containers using built-in Linux capabilities.

#### Integrate firejail with your desktop environment:
```shell
sudo firecfg
```
#### Open a restricted Mozilla Firefox:
```shell
firejail {{firefox}}
```
#### Start a restricted Apache server on a known interface and address:
```shell
firejail --net={{eth0}} --ip={{192.168.1.244}} {{/etc/init.d/apache2}} {{start}}
```
#### List running sandboxes:
```shell
firejail --list
```
#### List network activity from running sandboxes:
```shell
firejail --netstats
```
#### Shutdown a running sandbox:
```shell
firejail --shutdown={{7777}}
```
{% endraw %}