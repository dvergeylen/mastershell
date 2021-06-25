---
layout: default
title: "passwd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="passwd">
  <a href="/en/common/passwd.html">passwd</a> <a href="#passwd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Passwd is a tool used to change a user's password.

#### Change the password of the current user interactively:
```shell
passwd
```
#### Change the password of a specific user:
```shell
passwd {{username}}
```
#### Get the current status of the user:
```shell
passwd -S
```
#### Make the password of the account blank (it will set the named account passwordless):
```shell
passwd -d
```
{% endraw %}