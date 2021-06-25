---
layout: default
title: "mongo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mongo">
  <a href="/pt_br/common/mongo.html">mongo</a> <a href="#mongo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cliente shell interativo de MongoDB.
> Mais informações: <https://docs.mongodb.com/manual/reference/program/mongo>.

#### Conectar a uma base de dados:
```shell
mongo {{base_de_dados}}
```
#### Conectar a uma base de dados em um host e porta específicos:
```shell
mongo --host {{host}} --port {{porta}} {{base_de_dados}}
```
#### Conectar a uma base de dados com um usuário específico, uma senha será pedida ao usuário:
```shell
mongo --username {{usuário}} {{base_de_dados}} --password
```
#### Avaliar JavaScript na base de dados:
```shell
mongo --eval '{{JSON.stringify(db.foo.findOne())}}' {{base_de_dados}}
```
{% endraw %}