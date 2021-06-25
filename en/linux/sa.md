---
layout: default
title: "sa"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sa">
  <a href="/en/linux/sa.html">sa</a> <a href="#sa"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Summarizes accounting information. Part of the acct package.
> Shows commands called by users, including basic info on CPU time spent processing and I/O rates.

#### Display executable invocations per user (username not displayed):
```shell
sudo sa
```
#### Display executable invocations per user, showing responsible usernames:
```shell
sudo sa --print-users
```
#### List resources used recently per user:
```shell
sudo sa --user-summary
```
{% endraw %}