---
layout: default
title: "brew"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="brew">
  <a href="/pt_br/linux/brew.html">brew</a> <a href="#brew"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A versão Linux do gerenciador de pacotes Homebrew.

#### Buscar por fórmulas disponíveis:
```shell
brew search {{termo_da_busca}}
```
#### Instalar a última versão estável de uma fórmula (utilizar `--devel` para versões de desenvolvimento):
```shell
brew install {{formula}}
```
#### Listar as fórmulas instaladas:
```shell
brew list
```
#### Atualizar uma fórmula instalada (se não for informado o nome de uma fórmula, todas as fórmulas serão atualizadas):
```shell
brew upgrade {{formula}}
```
#### Recuperar a versão mais recente do Linuxbrew e de todas as fórmulas do GitHub:
```shell
brew update
```
#### Exibir as fórmulas que possuem novas versões disponíveis:
```shell
brew outdated
```
#### Exibir informações sobre uma fórmula (versão, caminho de instalação, dependências, etc.):
```shell
brew info {{formula}}
```
#### Verificar a instalação local em busca de possíveis problemas:
```shell
brew doctor
```
{% endraw %}