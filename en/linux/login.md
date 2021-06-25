---
layout: default
title: "login"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="login">
  <a href="/en/linux/login.html">login</a> <a href="#login"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Initiates a session for a user.

#### Log in as a user:
```shell
login {{user}}
```
#### Log in as user without authentication if user is preauthenticated:
```shell
login -f {{user}}
```
#### Log in as user and preserve environment:
```shell
login -p {{user}}
```
#### Log in as a user on a remote host:
```shell
login -h {{host}} {{user}}
```
{% endraw %}