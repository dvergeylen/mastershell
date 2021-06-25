---
layout: default
title: "su"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="su">
  <a href="/en/common/su.html">su</a> <a href="#su"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Switch shell to another user.

#### Switch to superuser (requires the root password):
```shell
su
```
#### Switch to a given user (requires the user's password):
```shell
su {{username}}
```
#### Switch to a given user and simulate a full login shell:
```shell
su - {{username}}
```
#### Execute a command as another user:
```shell
su - {{username}} -c "{{command}}"
```
{% endraw %}