---
layout: default
title: "mysql"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mysql">
  <a href="/pt_br/common/mysql.html">mysql</a> <a href="#mysql"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A ferramenta de linha de comando do MySQL.
> Mais informações: <https://www.mysql.com/>.

#### Conectar a um banco de dados:
```shell
mysql {{nome_do_banco_de_dados}}
```
#### Conectar a um banco de dados (será solicitada a senha de acesso do usuário):
```shell
mysql -u {{usuário}} --password {{nome_do_banco_de_dados}}
```
#### Conectar a um banco de dados disponível em um endereço específico:
```shell
mysql -h {{endereco_do_banco_de_dados}} {{nome_do_banco_de_dados}}
```
#### Conectar a um banco de dados utilizando um socket Unix:
```shell
mysql --socket {{caminho/para/socket.sock}}
```
#### Executar todos os comandos de um arquivo SQL em um banco de dados:
```shell
mysql -e "source {{nome_do_arquivo.sql}}" {{nome_do_banco_de_dados}}
```
{% endraw %}