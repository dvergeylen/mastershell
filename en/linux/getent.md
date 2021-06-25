---
layout: default
title: "getent"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="getent">
  <a href="/en/linux/getent.html">getent</a> <a href="#getent"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get entries from Name Service Switch libraries.

#### Get list of all groups:
```shell
getent group
```
#### See the members of a group:
```shell
getent group {{group_name}}
```
#### Get list of all services:
```shell
getent services
```
#### Find a username by UID:
```shell
getent passwd 1000
```
#### Perform a reverse DNS lookup:
```shell
getent hosts {{host}}
```
{% endraw %}