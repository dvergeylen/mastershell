---
layout: default
title: "pg_dump"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pg_dump">
  <a href="/en/common/pg_dump.html">pg_dump</a> <a href="#pg_dump"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Extract a PostgreSQL database into a script file or other archive file.
> More information: <https://www.postgresql.org/docs/current/app-pgdump.html>.

#### Dump database into a SQL-script file:
```shell
pg_dump {{db_name}} > {{output_file.sql}}
```
#### Same as above, customize username:
```shell
pg_dump -U {{username}} {{db_name}} > {{output_file.sql}}
```
#### Same as above, customize host and port:
```shell
pg_dump -h {{host}} -p {{port}} {{db_name}} > {{output_file.sql}}
```
#### Dump a database into a custom-format archive file:
```shell
pg_dump -Fc {{db_name}} > {{output_file.dump}}
```
#### Dump only database data into an SQL-script file:
```shell
pg_dump -a {{db_name}} > {{path/to/output_file.sql}}
```
#### Dump only schema (data definitions) into an SQL-script file:
```shell
pg_dump -s {{db_name}} > {{path/to/output_file.sql}}
```
{% endraw %}