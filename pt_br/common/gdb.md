---
layout: default
title: "gdb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gdb">
  <a href="/pt_br/common/gdb.html">gdb</a> <a href="#gdb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> O depurador GNU.
> Mais informações: <https://www.gnu.org/software/gdb>.

#### Depurar um executável:
```shell
gdb {{executável}}
```
#### Vincular um processo ao gdb:
```shell
gdb -p {{PID}}
```
#### Depurar usando um arquivo de "core dump":
```shell
gdb -c {{core}} {{executável}}
```
#### Executa um dado comando do gdb ao iniciar:
```shell
gdb -ex "{{comandos}}" {{executável}}
```
#### Inicia o gdb passando argumentos para o executável:
```shell
gdb --args {{executável}} {{argumento1}} {{argumento2}}
```
{% endraw %}