---
layout: default
title: "bundle"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bundle">
  <a href="/pt_br/common/bundle.html">bundle</a> <a href="#bundle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciador de dependências da linguagem de programação Ruby.
> Mais informações: <https://bundler.io/man/bundle.1.html>.

#### Instalar todas as gemas definidas no `Gemfile`:
```shell
bundle install
```
#### Atualizar todas as gemas, respeitando as regras definidas no `Gemfile`, e recriar o arquivo `Gemfile.lock`:
```shell
bundle update
```
#### Atualizar uma gema específica definida no `Gemfile`:
```shell
bundle update --source {{nome_da_gema}}
```
#### Criar o esqueleto do projeto de uma nova gema:
```shell
bundle gem {{nome_da_gema}}
```
{% endraw %}