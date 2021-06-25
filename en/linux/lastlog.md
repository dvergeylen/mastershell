---
layout: default
title: "lastlog"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lastlog">
  <a href="/en/linux/lastlog.html">lastlog</a> <a href="#lastlog"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show the most recent login of all users or of a given user.

#### Display the most recent login of all users:
```shell
lastlog
```
#### Display lastlog record of the specified user:
```shell
lastlog -u {{username}}
```
#### Display records before than 7 days:
```shell
lastlog -b {{7}}
```
#### Display records more recent than 3 days:
```shell
lastlog -t {{3}}
```
{% endraw %}