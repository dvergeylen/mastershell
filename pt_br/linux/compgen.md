---
layout: default
title: "compgen"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="compgen">
  <a href="/pt_br/linux/compgen.html">compgen</a> <a href="#compgen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Um programa para auto completar comandos no Bash, ele é executado ao pressionar duas vezes a tecla TAB.

#### Exibir todos os comandos que você pode executar:
```shell
compgen -c
```
#### Exibir todos os alias:
```shell
compgen -a
```
#### Exibir todas as funções que você pode executar:
```shell
compgen -A function
```
#### Exibir todas as palavras reservadas do shell:
```shell
compgen -k
```
#### Exibir todos os comandos/alias que iniciam com o termo 'ls':
```shell
compgen -ac {{ls}}
```
{% endraw %}