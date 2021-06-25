---
layout: default
title: "rails"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rails">
  <a href="/pt_br/common/rails.html">rails</a> <a href="#rails"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Framework MVC para o desenvolvimento de aplicações web, desenvolvido em Ruby.
> Mais informações: <https://guides.rubyonrails.org/command_line.html>.

#### Criar um novo projeto:
```shell
rails new "{{nome_do_projeto}}"
```
#### Iniciar o servidor local para o projeto atual na porta 3000:
```shell
rails server
```
#### Iniciar o servidor local para o projeto atual em um porta específica:
```shell
rails server -p "{{porta}}"
```
#### Iniciar o console Rails para manipular o projeto atual utilizando o terminal:
```shell
rails console
```
#### Verificar a versão atual do Rails:
```shell
rails --version
```
{% endraw %}