---
layout: default
title: "choco install"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-install">
  <a href="/pt_br/windows/choco-install.html">choco install</a> <a href="#choco-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Instalar um pacote ou mais com Chocolatey.
> Mais informações: <https://chocolatey.org/docs/commands-install>.

#### Instalar um ou mais pacotes separado por espaço:
```shell
choco install {{pacote(s)}}
```
#### Instalar pacotes a partir de um aquivo de configuração personalizado:
```shell
choco install {{caminho/para/pacotes.config}}
```
#### Instalar um arquivo específico `nuspec` ou `nupkg`:
```shell
choco install {{caminho/para/arquivo}}
```
#### Instalar uma versão específica de um pacote:
```shell
choco install {{pacote}} --version {{versão}}
```
#### Permitir a instalação de múltiplas versões de um pacote:
```shell
choco install {{pacote}} --allow-multiple
```
#### Confirmar todos prompts automaticamente:
```shell
choco install {{pacote}} --yes
```
#### Especificar uma fonte personalizada para receber pacotes:
```shell
choco install {{pacote}} --source {{url_do_pacote|apelido}}
```
#### Fornecer um nome e uma senha para autenticação:
```shell
choco install {{pacote}} --user {{usuario}} --password {{senha}}
```
{% endraw %}