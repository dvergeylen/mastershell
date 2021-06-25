---
layout: default
title: "choco uninstall"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-uninstall">
  <a href="/pt_br/windows/choco-uninstall.html">choco uninstall</a> <a href="#choco-uninstall"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Desinstalar um pacote ou mais com Chocolatey.
> Mais informações: <https://chocolatey.org/docs/commands-uninstall>.

#### Desinstalar um pacote ou mais separado por espaços:
```shell
choco uninstall {{pacote(s)}}
```
#### Desinstalar uma versão específica de um pacote:
```shell
choco uninstall {{pacote}} --version {{versão}}
```
#### Confirmar todos prompts automaticamente:
```shell
choco uninstall {{pacote}} --yes
```
#### Remover todas dependências ao desinstalar:
```shell
choco uninstall {{pacote}} --remove-dependencies
```
#### Desinstalar todos os pacotes:
```shell
choco uninstall all
```
{% endraw %}