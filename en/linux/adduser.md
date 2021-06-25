---
layout: default
title: "adduser"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adduser">
  <a href="/en/linux/adduser.html">adduser</a> <a href="#adduser"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> User addition utility.
> More information: <https://manpages.debian.org/latest/adduser/adduser.html>.

#### Create a new user with a default home directory and prompt the user to set a password:
```shell
adduser {{username}}
```
#### Create a new user without a home directory:
```shell
adduser --no-create-home {{username}}
```
#### Create a new user with a home directory at the specified path:
```shell
adduser --home {{path/to/home}} {{username}}
```
#### Create a new user with the specified shell set as the login shell:
```shell
adduser --shell {{path/to/shell}} {{username}}
```
#### Create a new user belonging to the specified group:
```shell
adduser --ingroup {{group}} {{username}}
```
#### Add an existing user to the specified group:
```shell
adduser {{username}} {{group}}
```
{% endraw %}