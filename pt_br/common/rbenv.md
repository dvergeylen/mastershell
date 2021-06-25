---
layout: default
title: "rbenv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rbenv">
  <a href="/pt_br/common/rbenv.html">rbenv</a> <a href="#rbenv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta que facilita a instalação e gerenciamento de múltiplas versões da linguagem Ruby.

#### Instalar uma ou mais versões, separadas por espaço:
```shell
rbenv install {{uma_ou_mais_versoes}}
```
#### Exibir a lista de versões instaladas:
```shell
rbenv versions
```
#### Determinar uma versão específica para ser a instalação padrão:
```shell
rbenv global {{versao}}
```
#### Determinar uma versão específica para um projeto. Este comando deve ser executado no diretório do projeto:
```shell
rbenv local {{versao}}
```
#### Exibir a versão ativa:
```shell
rbenv version
```
#### Remover uma versão:
```shell
rbenv uninstall {{versao}}
```
#### Exibir todas as versões que contém um determinado executável:
```shell
rbenv whence {{executavel}}
```
{% endraw %}