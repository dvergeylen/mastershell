---
layout: default
title: "mongo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mongo">
  <a href="/en/common/mongo.html">mongo</a> <a href="#mongo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> MongoDB interactive shell client.
> More information: <https://docs.mongodb.com/manual/reference/program/mongo>.

#### Connect to a database:
```shell
mongo {{database}}
```
#### Connect to a database running on a given host on a given port:
```shell
mongo --host {{host}} --port {{port}} {{database}}
```
#### Connect to a database with a given username; user will be prompted for password:
```shell
mongo --username {{username}} {{database}} --password
```
#### Evaluate a JavaScript expression on the database:
```shell
mongo --eval '{{JSON.stringify(db.foo.findOne())}}' {{database}}
```
{% endraw %}