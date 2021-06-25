---
layout: default
title: "mysqldump"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mysqldump">
  <a href="/pt_br/common/mysqldump.html">mysqldump</a> <a href="#mysqldump"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Realizar e restaurar backups no MySQL.
> Mais informações: <https://dev.mysql.com/doc/refman/en/mysqldump.html>.

#### Criar o backup do banco de dados em arquivo de saída (será solicitada a senha de acesso do usuário):
```shell
mysqldump -u {{usuário}} --password {{nome_do_banco_de_dados}} -r {{arquivo_de_saida.sql}}
```
#### Restaurar o conteúdo contido no arquivo de backup em banco de dados específico (será solicitada a senha de acesso do usuário):
```shell
mysql -u {{usuário}} --password -e "source {{arquivo_de_backup.sql}}" {{nome_do_banco_de_dados}}
```
{% endraw %}