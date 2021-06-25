---
layout: default
title: "cradle sql"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cradle-sql">
  <a href="/en/common/cradle-sql.html">cradle sql</a> <a href="#cradle-sql"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage Cradle SQL databases.
> More information: <https://cradlephp.github.io/docs/3.B.-Reference-Command-Line-Tools.html#sql>.

#### Rebuild the database schema:
```shell
cradle sql build
```
#### Rebuild the database schema for a specific package:
```shell
cradle sql build {{package_name}}
```
#### Empty the entire database:
```shell
cradle sql flush
```
#### Empty the database tables for a specific package:
```shell
cradle sql flush {{package_name}}
```
#### Populate the tables for all packages:
```shell
cradle sql populate
```
#### Populate the tables for a specific package:
```shell
cradle sql populate {{package_name}}
```
{% endraw %}