---
layout: default
title: "pg_restore"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pg_restore">
  <a href="/en/common/pg_restore.html">pg_restore</a> <a href="#pg_restore"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Restore a PostgreSQL database from an archive file created by pg_dump.
> More information: <https://www.postgresql.org/docs/current/app-pgrestore.html>.

#### Restore an archive into an existing database:
```shell
pg_restore -d {{db_name}} {{archive_file.dump}}
```
#### Same as above, customize username:
```shell
pg_restore -U {{username}} -d {{db_name}} {{archive_file.dump}}
```
#### Same as above, customize host and port:
```shell
pg_restore -h {{host}} -p {{port}} -d {{db_name}} {{archive_file.dump}}
```
#### List database objects included in the archive:
```shell
pg_restore --list {{archive_file.dump}}
```
#### Clean database objects before creating them:
```shell
pg_restore --clean -d {{db_name}} {{archive_file.dump}}
```
#### Use multiple jobs to do the restoring:
```shell
pg_restore -j {{2}} -d {{db_name}} {{archive_file.dump}}
```
{% endraw %}