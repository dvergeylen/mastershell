---
layout: default
title: "mysqld"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mysqld">
  <a href="/en/common/mysqld.html">mysqld</a> <a href="#mysqld"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Start the MySQL database server.
> More information: <https://dev.mysql.com/doc/refman/en/mysqld.html>.

#### Start the MySQL database server:
```shell
mysqld
```
#### Start the server, printing error messages to the console:
```shell
mysqld --console
```
#### Start the server, saving logging output to a custom log file:
```shell
mysqld --log={{path/to/file.log}}
```
#### Print the default arguments and their values and exit:
```shell
mysqld --print-defaults
```
#### Start the server, reading arguments and values from a file:
```shell
mysqld --defaults-file={{path/to/file}}
```
#### Start the server and listen on a custom port:
```shell
mysqld --port={{port}}
```
#### Show all help options and exit:
```shell
mysqld --verbose --help
```
{% endraw %}