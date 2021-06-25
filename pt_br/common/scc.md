---
layout: default
title: "scc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="scc">
  <a href="/pt_br/common/scc.html">scc</a> <a href="#scc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilitário escrito em GO que conta linhas de código.
> Mais informações: <https://github.com/boyter/scc>.

#### Mostrar o número de linhas de código no diretório atual:
```shell
scc
```
#### Mostrar o número de linhas de código de um diretório especificado:
```shell
scc {{caminho/para/diretorio}}
```
#### Mostrar o número de linhas de código por arquivo:
```shell
scc --by-file
```
#### Mostrar o resultado usando um formato específico (formato padrão é o `tabular`):
```shell
scc --format {{tabular|wide|json|csv|cloc-yaml|html|html-table}}
```
#### Contar apenas os arquivos com as extensões especificadas:
```shell
scc --include-ext {{go, java, js}}
```
#### Excluir diretórios da contagem:
```shell
scc --exclude-dir {{.git,.hg}}
```
#### Mostrar output organizado de acordo com o parâmetro especificado (organização padrão é `files`):
```shell
scc --sort {{files|name|lines|blanks|code|comments|complexity}}
```
#### Mostra a tela de ajuda:
```shell
scc -h
```
{% endraw %}