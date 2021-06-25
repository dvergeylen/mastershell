---
layout: default
title: "rvm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rvm">
  <a href="/pt_br/common/rvm.html">rvm</a> <a href="#rvm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta que facilita a instalação e gerenciamento de múltiplas versões da linguagem Ruby.

#### Instalar uma ou mais versões separadas por espaço:
```shell
rvm install {{uma_ou_mais_versoes}}
```
#### Exibir a lista de versões instaladas:
```shell
rvm list
```
#### Definir uma versão específica para ser utilizada temporariamente:
```shell
rvm use {{versao}}
```
#### Definir uma versão específica para ser a instalação padrão:
```shell
rvm --default use {{versao}}
```
#### Atualizar uma versão já instalada para uma nova versão:
```shell
rvm upgrade {{versao_atual}} {{nova_versao}}
```
#### Remover uma versão mantendo o código fonte:
```shell
rvm uninstall {{versao}}
```
#### Remover uma versão e o código fonte:
```shell
rvm remove {{versao}}
```
#### Exibir as dependências específicas para o seu sistema operacional:
```shell
rvm requirements
```
{% endraw %}