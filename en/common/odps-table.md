---
layout: default
title: "odps table"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="odps-table">
  <a href="/en/common/odps-table.html">odps table</a> <a href="#odps-table"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create and modify tables in ODPS (Open Data Processing Service).
> See also `odps`.
> More information: <https://www.alibabacloud.com/help/doc-detail/27971.htm>.

#### Create a table with partition and lifecycle:
```shell
create table {{table_name}} ({{col}} {{type}}) partitioned by ({{col}} {{type}}) lifecycle {{days}};
```
#### Create a table based on the definition of another table:
```shell
create table {{table_name}} like {{another_table}};
```
#### Add partition to a table:
```shell
alter table {{table_name}} add partition ({{partition_spec}});
```
#### Delete partition from a table:
```shell
alter table {{table_name}} drop partition ({{partition_spec}});
```
#### Delete table:
```shell
drop table {{table_name}};
```
{% endraw %}