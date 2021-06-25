---
layout: default
title: "sequelize"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sequelize">
  <a href="/en/common/sequelize.html">sequelize</a> <a href="#sequelize"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Promise-based Node.js ORM for Postgres, MySQL, MariaDB, SQLite and Microsoft SQL Server.
> More information: <https://sequelize.org/>.

#### Create a model with 3 fields and a migration file:
```shell
sequelize model:generate --name {{table_name}} --attributes {{field1:integer,field2:string,field3:boolean}}
```
#### Run the migration file:
```shell
sequelize db:migrate
```
#### Revert all migrations:
```shell
sequelize db:migrate:undo:all
```
#### Create a seed file with the specified name to populate the database:
```shell
sequelize seed:generate --name {{seed_filename}}
```
#### Populate database using all seed files:
```shell
sequelize db:seed:all
```
{% endraw %}