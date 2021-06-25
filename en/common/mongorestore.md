---
layout: default
title: "mongorestore"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mongorestore">
  <a href="/en/common/mongorestore.html">mongorestore</a> <a href="#mongorestore"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to import a collection or database from a binary dump into a MongoDB instance.
> More information: <https://docs.mongodb.com/database-tools/mongorestore/>.

#### Import a bson data dump from a directory to a MongoDB database:
```shell
mongorestore --db {{database_name}} {{path/to/directory}}
```
#### Import a bson data dump from a directory to a given database in a MongoDB server host, running at a given port, with user authentication (user will be prompted for password):
```shell
mongorestore --host {{database_host:port}} --db {{database_name}} --username {{username}} {{path/to/directory}} --password
```
#### Import a collection from a bson file to a MongoDB database:
```shell
mongorestore --db {{database_name}} {{path/to/file}}
```
#### Import a collection from a bson file to a given database in a MongoDB server host, running at a given port, with user authentication (user will be prompted for password):
```shell
mongorestore --host {{database_host:port}} --db {{database_name}} --username {{username}} {{path/to/file}} --password
```
{% endraw %}