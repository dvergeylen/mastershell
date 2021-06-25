---
layout: default
title: "lastb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lastb">
  <a href="/en/linux/lastb.html">lastb</a> <a href="#lastb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show a listing of last logged in users.

#### Show a list of all last logged in users:
```shell
sudo lastb
```
#### Show a list of all last logged in users since a given time:
```shell
sudo lastb --since {{YYYY-MM-DD}}
```
#### Show a list of all last logged in users until a given time:
```shell
sudo lastb --until {{YYYY-MM-DD}}
```
#### Show a list of all logged in users at a specific time:
```shell
sudo lastb --present {{hh:mm}}
```
#### Show a list of all last logged in users and translate the IP into a hostname:
```shell
sudo lastb --dns
```
{% endraw %}