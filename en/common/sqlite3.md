---
layout: default
title: "sqlite3"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sqlite3">
  <a href="/en/common/sqlite3.html">sqlite3</a> <a href="#sqlite3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The command-line interface to SQLite 3, which is a self-contained file-based embedded SQL engine.
> More information: <https://sqlite.org>.

#### Start an interactive shell with a new database:
```shell
sqlite3
```
#### Open an interactive shell against an existing database:
```shell
sqlite3 {{path/to/database.sqlite3}}
```
#### Execute an SQL statement against a database and then exit:
```shell
sqlite3 {{path/to/database.sqlite3}} '{{SELECT * FROM some_table;}}'
```
{% endraw %}