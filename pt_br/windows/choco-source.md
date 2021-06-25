---
layout: default
title: "choco source"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-source">
  <a href="/pt_br/windows/choco-source.html">choco source</a> <a href="#choco-source"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciar fontes para pacotes com Chocolatey.
> Mais informações: <https://chocolatey.org/docs/commands-source>.

#### Listar fontes atualmente disponíveis:
```shell
choco source list
```
#### Adicionar uma nova fonte de pacotes:
```shell
choco source add --name {{nome}} --source {{url_da_fonte}}
```
#### Adicionar uma nova fonte de pacotes com credenciais:
```shell
choco source add --name {{nome}} --source {{url_da_fonte}} --user {{nome}} --password {{senha}}
```
#### Adicionar uma nova fonte de pacotes com certificado do cliente:
```shell
choco source add --name {{nome}} --source {{url_da_fonte}} --cert {{caminho/para/certificado}}
```
#### Habilitar uma fonte de pacotes:
```shell
choco source enable --name {{nome}}
```
#### Desabilitar uma fonte de pacotes:
```shell
choco source disable --name {{nome}}
```
#### Remover uma fonte de pacotes:
```shell
choco source remove --name {{nome}}
```
{% endraw %}