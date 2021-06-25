---
layout: default
title: "mysqldump"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mysqldump">
  <a href="/en/common/mysqldump.html">mysqldump</a> <a href="#mysqldump"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Backups MySQL databases.
> See also `mysql` for restoring databases.
> More information: <https://dev.mysql.com/doc/refman/en/mysqldump.html>.

#### Create a backup (user will be prompted for a password):
```shell
mysqldump --user {{user}} --password {{database_name}} --result-file={{path/to/file.sql}}
```
#### Backup a specific table redirecting the output to a file (user will be prompted for a password):
```shell
mysqldump --user {{user}} --password {{database_name}} {{table_name}} > {{path/to/file.sql}}
```
#### Backup all databases redirecting the output to a file (user will be prompted for a password):
```shell
mysqldump --user {{user}} --password --all-databases > {{path/to/file.sql}}
```
#### Backup all databases from a remote host, redirecting the output to a file (user will be prompted for a password):
```shell
mysqldump --host={(ip_or_hostname)} --user {{user}} --password --all-databases > ({path/to/file.sql}}
```
{% endraw %}