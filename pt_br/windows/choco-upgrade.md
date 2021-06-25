---
layout: default
title: "choco upgrade"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-upgrade">
  <a href="/pt_br/windows/choco-upgrade.html">choco upgrade</a> <a href="#choco-upgrade"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Atualizar um ou mais pacotes com Chocolatey.
> Mais informações: <https://chocolatey.org/docs/commands-upgrade>.

#### Atualizar um ou mais pacotes separados por espaço:
```shell
choco upgrade {{pacote(s)}}
```
#### Atualizar para uma versão específica de um pacote:
```shell
choco upgrade {{pacote}} --version {{versão}}
```
#### Atualizar todos pacotes:
```shell
choco upgrade all
```
#### Atualizar todos os pacotes, exceto os especificados separados por virgula:
```shell
choco upgrade all --except "{{pacote(s)}}"
```
#### Confirmar todos prompts automaticamente:
```shell
choco upgrade {{pacote}} --yes
```
#### Especifique uma fonte personalizada para receber pacotes:
```shell
choco upgrade {{pacote}} --source {{url_do_pacote|apelido}}
```
#### Fornecer um nome e uma senha para autenticação:
```shell
choco upgrade {{pacote}} --user {{usuário}} --password {{senha}}
```
{% endraw %}