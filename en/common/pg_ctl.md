---
layout: default
title: "pg_ctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pg_ctl">
  <a href="/en/common/pg_ctl.html">pg_ctl</a> <a href="#pg_ctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility for controlling a PostgreSQL server and database cluster.
> More information: <https://www.postgresql.org/docs/current/app-pg-ctl.html>.

#### Initialize a new PostgreSQL database cluster:
```shell
pg_ctl -D {{data_directory}} init
```
#### Start a PostgreSQL server:
```shell
pg_ctl -D {{data_directory}} start
```
#### Stop a PostgreSQL server:
```shell
pg_ctl -D {{data_directory}} stop
```
#### Restart a PostgreSQL server:
```shell
pg_ctl -D {{data_directory}} restart
```
#### Reload the PostgreSQL server configuration:
```shell
pg_ctl -D {{data_directory}} reload
```
{% endraw %}