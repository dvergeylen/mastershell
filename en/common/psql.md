---
layout: default
title: "psql"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="psql">
  <a href="/en/common/psql.html">psql</a> <a href="#psql"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> PostgreSQL command-line client.
> More information: <https://www.postgresql.org/docs/current/app-psql.html>.

#### Connect to database. It connects to localhost using default port 5432 with default user as currently logged in user:
```shell
psql {{database}}
```
#### Connect to database on given server host running on given port with given username, without a password prompt:
```shell
psql -h {{host}} -p {{port}} -U {{username}} {{database}}
```
#### Connect to database; user will be prompted for password:
```shell
psql -h {{host}} -p {{port}} -U {{username}} -W {{database}}
```
#### Execute a single SQL query or PostgreSQL command on the given database (useful in shell scripts):
```shell
psql -c '{{query}}' {{database}}
```
#### Execute commands from a file on the given database:
```shell
psql {{database}} -f {{file.sql}}
```
{% endraw %}