---
layout: default
title: "gpasswd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gpasswd">
  <a href="/en/linux/gpasswd.html">gpasswd</a> <a href="#gpasswd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Administer `/etc/group` and `/etc/gshadow`.

#### Define group administrators:
```shell
sudo gpasswd -A {{user1,user2}} {{group}}
```
#### Set the list of group members:
```shell
sudo gpasswd -M {{user1,user2}} {{group}}
```
#### Create a password for the named group:
```shell
gpasswd {{group}}
```
#### Add a user to the named group:
```shell
gpasswd -a {{user}} {{group}}
```
#### Remove a user from the named group:
```shell
gpasswd -d {{user}} {{group}}
```
{% endraw %}