---
layout: default
title: "mysql"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mysql">
  <a href="/es/common/mysql.html">mysql</a> <a href="#mysql"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta de línea de comandos para gestionar bases de datos MySQL.
> Más información: <https://www.mysql.com/>.

#### Conecta a una base de datos:
```shell
mysql {{nombre_base_de_datos}}
```
#### Conecta a una base de datos con el usuario `usuario` y se le pedirá la contraseña:
```shell
mysql -u {{usuario}} --password {{nombre_base_de_datos}}
```
#### Conecta a una base de datos en otra máquina:
```shell
mysql -h {{maquina_remota}} {{nombre_base_de_datos}}
```
#### Conecta a una base de datos a través de un socket unix:
```shell
mysql --socket {{ruta/al/socket.sock}}
```
#### Ejecuta comandos SQL contenidos en un script:
```shell
mysql -e "source {{archivo.sql}}" {{nombre_base_de_datos}}
```
#### Restaura una base de datos a partir de una copia de seguridad creada con `mysqldump` (y se le pedirá la contraseña al usuario):
```shell
mysql --user {{usuario}} --password {{nombre_base_de_datos}} < {{ruta/al/backup.sql}}
```
#### Restaura todas las bases de datos en una copia de seguridad (y se le pedirá la contraseña al usuario):
```shell
mysql --user {{usuario}} --password < {{ruta/al/backup.sql}}
```
{% endraw %}