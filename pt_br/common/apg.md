---
layout: default
title: "apg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apg">
  <a href="/pt_br/common/apg.html">apg</a> <a href="#apg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Criar senhas aleatórias arbitrariamente complexas.
> Mais informações: <https://manned.org/apg>.

#### Criar senha aleatória (tamanho padrão para as senhas é 8 caracteres):
```shell
apg
```
#### Criar senha com pelo menos 1 símbolo (S), 1 número (N), 1 letra maiúscula (C), 1 letra minúscula (L):
```shell
apg -M SNCL
```
#### Criar uma senha com 16 caracteres:
```shell
apg -m {{16}}
```
#### Criar senha com tamanho máximo de 16 caracteres:
```shell
apg -x {{16}}
```
#### Criar uma senha que não aparece em um dicionário provido pelo usuário:
```shell
apg -r {{arquivo_de_dicionario}}
```
{% endraw %}