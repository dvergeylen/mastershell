---
layout: default
title: "choco list"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-list">
  <a href="/pt_br/windows/choco-list.html">choco list</a> <a href="#choco-list"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Exibir uma lista de pacotes com Chocolatey.
> Mais informações: <https://chocolatey.org/docs/commands-list>.

#### Exibir todos pacotes disponíveis:
```shell
choco list
```
#### Exibir todos pacotes instalados localmente:
```shell
choco list --local-only
```
#### Exibir uma lista incluindo programas locais:
```shell
choco list --include-programs
```
#### Exibir apenas pacotes aprovados:
```shell
choco list --approved-only
```
#### Especificar uma fonte personalizada para exibir os pacotes:
```shell
choco list --source {{url_da_fonte|apelido}}
```
#### Fornecer um nome e uma senha para autenticação:
```shell
choco list --user {{usuário}} --password {{senha}}
```
{% endraw %}