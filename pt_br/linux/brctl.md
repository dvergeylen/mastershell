---
layout: default
title: "brctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="brctl">
  <a href="/pt_br/linux/brctl.html">brctl</a> <a href="#brctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Administração de pontes de rede.

#### Exibir uma lista com informações das pontes de rede existentes:
```shell
sudo brctl show
```
#### Cria uma ponte de rede:
```shell
sudo brctl add {{nome_da_ponte}}
```
#### Remover uma ponte de rede:
```shell
sudo brctl del {{nome_da_ponte}}
```
#### Adicionar uma interface de rede em uma ponte de rede existente:
```shell
sudo brctl addif {{nome_da_ponte}} {{nome_da_interface_de_rede}}
```
#### Remover uma interface de rede de uma ponte de rede existente:
```shell
sudo brctl delif {{nome_da_ponte}} {{nome_da_interface_de_rede}}
```
{% endraw %}