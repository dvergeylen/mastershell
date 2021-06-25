---
layout: default
title: "rails generate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rails-generate">
  <a href="/pt_br/common/rails-generate.html">rails generate</a> <a href="#rails-generate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerar artefatos Rails a partir de um modelo em um projeto existente.

#### Exibir todos os geradores disponíveis:
```shell
rails generate
```
#### Criar um modelo:
```shell
rails generate model {{nome_da_classe}}
```
#### Criar um controlador:
```shell
rails generate controller {{nome_do_controlador}}
```
#### Criar uma estrutura completa (modelo, controlador, testes, etc.) para um novo modelo:
```shell
rails generate scaffold {{nome_do_modelo}}
```
{% endraw %}