---
layout: default
title: "cmus"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cmus">
  <a href="/pt_br/linux/cmus.html">cmus</a> <a href="#cmus"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Player de música via terminal.
> Use as setas para navegar, `<enter/return>` para selecionar, e números 1-8 para alterar as telas de opções.

#### Iniciar o cmus em um diretório específico:
```shell
cmus {{caminho_do_diretorio}}
```
#### Adicionar arquivo/diretório a biblioteca:
```shell
:add {{caminho_para_arquivo_ou_diretorio}}
```
#### Parar/reiniciar a música atual:
```shell
c
```
#### Ativar/Desativar o modo aleatório:
```shell
s
```
#### Sair cmus:
```shell
q
```
{% endraw %}