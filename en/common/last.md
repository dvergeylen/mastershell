---
layout: default
title: "last"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="last">
  <a href="/en/common/last.html">last</a> <a href="#last"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> View the last logged in users.

#### View last logins, their duration and other information as read from `/var/log/wtmp`:
```shell
last
```
#### Specify how many of the last logins to show:
```shell
last -n {{login_count}}
```
#### Print the full date and time for entries and then display the hostname column last to prevent truncation:
```shell
last -F -a
```
#### View all logins by a specific user and show the ip address instead of the hostname:
```shell
last {{username}} -i
```
#### View all recorded reboots (i.e., the last logins of the pseudo user "reboot"):
```shell
last reboot
```
#### View all recorded shutdowns (i.e., the last logins of the pseudo user "shutdown"):
```shell
last shutdown
```
{% endraw %}