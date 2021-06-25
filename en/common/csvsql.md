---
layout: default
title: "csvsql"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csvsql">
  <a href="/en/common/csvsql.html">csvsql</a> <a href="#csvsql"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate SQL statements for a CSV file or execute those statements directly on a database.
> Included in csvkit.
> More information: <https://csvkit.readthedocs.io/en/latest/scripts/csvsql.html>.

#### Generate a `CREATE TABLE` SQL statement for a CSV file:
```shell
csvsql {{path/to/data.csv}}
```
#### Import a CSV file into an SQL database:
```shell
csvsql --insert --db "{{mysql://user:password@host/database}}" {{data.csv}}
```
#### Run an SQL query on a CSV file:
```shell
csvsql --query "{{select * from 'data'}}" {{data.csv}}
```
{% endraw %}