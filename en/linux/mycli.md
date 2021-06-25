---
layout: default
title: "mycli"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mycli">
  <a href="/en/linux/mycli.html">mycli</a> <a href="#mycli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A CLI for MySQL, MariaDB, and Percona with auto-completion and syntax highlighting.

#### Connect to a database with the currently logged in user:
```shell
mycli {{database_name}}
```
#### Connect to a database with the specified user:
```shell
mycli -u {{user}} {{database_name}}
```
#### Connect to a database on the specified host with the specified user:
```shell
mycli -u {{user}} -h {{host}} {{database_name}}
```
{% endraw %}