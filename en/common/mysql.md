---
layout: default
title: "mysql"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mysql">
  <a href="/en/common/mysql.html">mysql</a> <a href="#mysql"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The MySQL command-line tool.
> More information: <https://www.mysql.com/>.

#### Connect to a database:
```shell
mysql {{database_name}}
```
#### Connect to a database, user will be prompted for a password:
```shell
mysql -u {{user}} --password {{database_name}}
```
#### Connect to a database on another host:
```shell
mysql -h {{database_host}} {{database_name}}
```
#### Connect to a database through a Unix socket:
```shell
mysql --socket {{path/to/socket.sock}}
```
#### Execute SQL statements in a script file (batch file):
```shell
mysql -e "source {{filename.sql}}" {{database_name}}
```
#### Restore a database from a backup created with `mysqldump` (user will be prompted for a password):
```shell
mysql --user {{user}} --password {{database_name}} < {{path/to/backup.sql}}
```
#### Restore all databases from a backup (user will be prompted for a password):
```shell
mysql --user {{user}} --password < {{path/to/backup.sql}}
```
{% endraw %}