---
layout: default
title: "add-apt-repository"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="add-apt-repository">
  <a href="/pt_br/linux/add-apt-repository.html">add-apt-repository</a> <a href="#add-apt-repository"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciar definições de repositórios APT.

#### Adicionar um repositório:
```shell
add-apt-repository {{especificacao_do_repositorio}}
```
#### Remover um repositório:
```shell
add-apt-repository --remove {{especificacao_do_repositorio}}
```
#### Adicionar um repositório e atualizar o cache do(s) pacote(s) deste repositório:
```shell
add-apt-repository --update {{especificacao_do_repositorio}}
```
#### Adicionar um repositório e habilitar o download do código fonte do(s) pacote(s) deste repositório:
```shell
add-apt-repository --enable-source {{especificacao_do_repositorio}}
```
{% endraw %}