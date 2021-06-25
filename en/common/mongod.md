---
layout: default
title: "mongod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mongod">
  <a href="/en/common/mongod.html">mongod</a> <a href="#mongod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The MongoDB database server.
> More information: <https://docs.mongodb.com/manual/reference/program/mongod>.

#### Specify a config file:
```shell
mongod --config {{filename}}
```
#### Specify the port to listen on:
```shell
mongod --port {{port}}
```
#### Specify database profiling level. 0 is off, 1 is only slow operations, 2 is all:
```shell
mongod --profile {{0|1|2}}
```
{% endraw %}