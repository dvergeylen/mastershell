---
layout: default
title: "lsof"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lsof">
  <a href="/pt_br/common/lsof.html">lsof</a> <a href="#lsof"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lista arquivos abertos e os seus processos correspondentes.
> Nota: Privilégios de administrador (ou sudo) são necessários para listar arquivos abertos por outros.

#### Localizar os processos que têm um certo arquivo aberto:
```shell
lsof {{caminho/para/arquivo}}
```
#### Localizar o processo que abriu uma porta de internet local:
```shell
lsof -i :{{porta}}
```
#### Mostrar o ID (PID) do processo que abriu um arquivo especificado:
```shell
lsof -t {{caminho/para/arquivo}}
```
#### Listar arquivos abertos por um certo usuário:
```shell
lsof -u {{nome_usuario}}
```
#### Listar arquivos abertos por um certo comando ou processo:
```shell
lsof -c {{nome_processo_ou_comando}}
```
#### Listar arquivos abertos por um certo processo, dado o seu PID:
```shell
lsof -p {{PID}}
```
#### Listar arquivos abertos em um diretório:
```shell
lsof +D {{caminho/para/diretório}}
```
#### Encontrar o processo que está ouvindo uma porta de TCP local:
```shell
lsof -iTCP:{{porta}} -sTCP:LISTEN
```
{% endraw %}