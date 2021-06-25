---
layout: default
title: "aspell"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aspell">
  <a href="/pt_br/linux/aspell.html">aspell</a> <a href="#aspell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verificador ortográfico interativo.

#### Verificar a ortografia do texto de um arquivo:
```shell
aspell check {{arquivo}}
```
#### Exibir as palavras escritas incorretamente no terminal:
```shell
cat {{arquivo}} | aspell list
```
#### Exibir os dicionários disponíveis:
```shell
aspell dicts
```
#### Executar aspell utilizando uma língua diferente (informe o código ISO 639 da língua):
```shell
aspell --lang={{cs}}
```
#### Exibir os erros ortográficos no terminal e ignorando as palavras da lista pessoal:
```shell
cat {{arquivo}} | aspell --personal={{lista_pessoal.pws}} {{list}}
```
{% endraw %}