---
layout: default
title: "batch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="batch">
  <a href="/pt_pt/common/batch.html">batch</a> <a href="#batch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Executar comandos num momento mais tarde quando a carga do sistema permitir.
> O serviço atd (ou atrun) deve correr para atuais execuções.
> Mais informações: <https://man.archlinux.org/man/at.1>.

#### Executar comandos da entrada padrão (premir `Ctrl + D` quando terminado):
```shell
batch
```
#### Executar um comando da entrada padrão:
```shell
echo "{{./criar_copia_bd.sh}}" | batch
```
#### Executar comandos de um dado ficheiro:
```shell
batch -f {{caminho/para/ficheiro}}
```
{% endraw %}